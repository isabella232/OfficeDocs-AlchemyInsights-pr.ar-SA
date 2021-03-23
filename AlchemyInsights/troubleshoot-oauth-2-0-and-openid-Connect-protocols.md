---
title: استكشاف الأخطاء في بروتوكولات OAuth 2.0 و OpenID Connect وإصلاحها
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9776"
- "9004342"
ms.openlocfilehash: d2f14d4d16bea890b564cdb9bd9ac3875c28d115
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51034832"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>استكشاف الأخطاء في بروتوكولات OAuth 2.0 و OpenID Connect وإصلاحها

لحل مشاكل OAuth 2.0 و OpenID Connect، قم بتنفيذ الخطوات التالية الموصى بها:

راجع المقالات التالية المتعلقة بالتكوين وإصلاح بروتوكولات OAuth 2.0 و OpenID Connect:

- النظام الأساسي لهوية Microsoft وتدفق رمز [التخويل OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) - تصف هذه المقالة كيفية البرمجة مباشرة مقابل تدفق منح التعليمات البرمجية **(PKCE)** في تطبيقك، باستخدام أي لغة.
- النظام الأساسي لهوية Microsoft وتدفق بيانات اعتماد [عميل OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) - تصف هذه المقالة كيفية البرمجة مباشرة مقابل تدفق بيانات اعتماد العميل **في** التطبيق.
- النظام الأساسي لهوية Microsoft وبيانات اعتماد كلمة مرور [مالك الموارد ل OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) - تصف هذه المقالة كيفية البرمجة مباشرة مقابل تدفق **ROPC** في التطبيق.
    - يدعم النظام الأساسي هوية Microsoft فقط ROPC لمستأجري Azure AD، وليس للحسابات الشخصية. وهذا يعني أنه يجب استخدام نقطة نهاية خاصة ب المستأجر **( https://login.microsoftonline.com/{TenantId_or_Name})** أو نقطة **نهاية** المؤسسات.
    - لا يمكن للحسابات الشخصية التي يتم دعوتها إلى مستأجر Azure AD استخدام ROPC.
    - لا يمكن للحسابات التي لا تملك كلمات مرور تسجيل الدخول عبر ROPC. في هذا السيناريو، نوصي باستخدام تدفق مختلف لتطبيقك، بدلا من ذلك.
    - إذا احتاج المستخدمون إلى استخدام المصادقة متعددة العوامل [(MFA)](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) لتسجيل الدخول إلى التطبيق، سيتم حظرهم.
    - ROPC غير معتمد [](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) في سيناريوهات اتحاد الهويات المختلطة (على سبيل المثال، Azure AD و ADFS المستخدمين لمصادقة الحسابات المحلي). إذا تمت إعادة توجيه المستخدمين في صفحة كاملة إلى موفر هوية في الموقع، لن يتمكن Azure AD من اختبار اسم المستخدم وكلمة المرور مقابل موفر الهوية هذا. [ومع ذلك، فإن المصادقة](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) المرورية معتمدة مع ROPC.
    - سيكون الاستثناء الوحيد لسيناريوهات اتحاد الهويات المختلطة هو ما يلي: سيمكن نهج "اكتشاف المجال المنزلي" مع تعيين **AllowCloudPasswordValidation** إلى **TRUE** تدفق ROPC للعمل للمستخدمين المتحدة عند مزامنة كلمة المرور المحلي إلى السحابة. لمزيد من المعلومات، راجع تمكين مصادقة [ROPC المباشرة](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications) للمستخدمين المتحدة للتطبيقات القديمة 
- النظام الأساسي لهوية [Microsoft وOAuth 2.0 On-Behalf-Of flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) - تصف هذه المقالة كيفية البرنامج مباشرة مقابل التدفق نيابة عن **(OBO)** في التطبيق.
- [النظام الأساسي لهوية Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) وبروتوكول OpenID Connect - توضح هذه المقالة كيفية تنفيذ بروتوكول OpenID Connect بشكل مستقل عن اللغة، كما تصف كيفية إرسال رسائل HTTP وتلقيها دون استخدام أي مكتبات Microsoft مفتوحة المصدر.

**رموز Access المميزة**

[الرموز المميزة للوصول إلى النظام](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) الأساسي ل Microsoft identity - تعرف على كيفية التحقق من صحة API واستخدام المطالبات داخل رمز الوصول المميز. تنطبق كل الوثائق في هذه المقالة، باستثناء الوثائق التي تم ذكرها، فقط على الرموز المميزة التي تم إصدارها ل واجهات برمجة التطبيقات التي قمت بتسجيلها. ولا ينطبق على الرموز المميزة التي تم إصدارها ل واجهات برمجة التطبيقات المملوكة ل Microsoft، ولا يمكن استخدام هذه الرموز المميزة للتحقق من كيفية إصدار النظام الأساسي لهوية Microsoft الرموز المميزة ل API التي تقوم بإنشاءها.

**تكوين التطبيق**

قيود وقيود إعادة توجيه [URI (عنوان URL للرد)](https://docs.microsoft.com/azure/active-directory/develop/reply-url) - تعرف على كيفية تكوين عنوان URL إعادة توجيه (URL للرد). عنوان URL لإعادة التوجيه أو عنوان URL للرد هو الموقع حيث يرسل خادم التخويل المستخدم بمجرد أن يتم تخويل التطبيق ومنحه رمز تخويل أو رمز وصول مميز بنجاح. يرسل خادم التخويل الرمز أو الرمز المميز إلى URI إعادة التوجيه؛ لذلك من المهم تسجيل الموقع الصحيح كجزء من عملية تسجيل التطبيق.

**توفير التطبيق**

[البرنامج التعليمي: تطوير وتوفير](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) خطة لنقطة نهاية SCIM - تصف هذه المقالة كيفية إنشاء نقطة نهاية SCIM والتكامل مع خدمة توفير AAD.


