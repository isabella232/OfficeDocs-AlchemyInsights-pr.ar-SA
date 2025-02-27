---
title: المشاكل المتعلقة باستخدام بيانات الاعتماد
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004330"
- "7723"
ms.openlocfilehash: 975d4850c1ecffae786dd19b7f4363e0c95378cff4f3ae6bb1968af33ef810b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986806"
---
# <a name="issues-with-credentials"></a>المشاكل المتعلقة باستخدام بيانات الاعتماد

النظام الأساسي للهويات في Microsoft بيانات اعتماد عميل [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) كيفية البرمجة مباشرة مقابل تدفق منح بيانات اعتماد عميل OAuth 2.0.

**كيف يمكنني إدارة كلمة مرور التطبيق أو بيانات اعتماد الشهادة؟**

في Azure CLI، يمكنك استخدام بيانات اعتماد تطبيق [az ad](https://docs.microsoft.com/cli/azure/ad/app/credential) لحذف كلمة مرور التطبيق أو بيانات اعتماد الشهادة أو سردها أو إعادة تعيينها.

**كيف يمكن للمستخدمين إعادة تعيين كلمات المرور الخاصة بهم؟**

يحتاج المستخدمون [إلى التسجيل لإعادة تعيين](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) كلمة المرور للخدمة الذاتية قبل أن يستطيعوا إعادة تعيين كلمات المرور الخاصة بهم. بمجرد تسجيل المستخدم، يمكنه اتباع الإرشادات الواردة في هذه المقالة لإعادة تعيين كلمة المرور الخاصة به: إعادة تعيين كلمة مرور العمل [أو المدرسة](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).

**كيف يمكن للمستخدمين تغيير كلمات المرور الخاصة بهم؟**

يمكن للمستخدمين اتباع الخطوات في هذه المقالة لتغيير كلمات المرور الخاصة بهم: [كيفية تغيير كلمة المرور](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)الخاصة بك .
يمكنهم أيضا [إدارة كلمات مرور التطبيق للتحقق على خطوتين](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).

**يحصل المستخدم على خطأ عند تغيير كلمة المرور أو إعادة تعيينها**

سيوفر هذا الارتباط معلومات حول المشاكل الشائعة التي قد تنشأ عندما يحاول المستخدم إعادة تعيين كلمة المرور الخاصة به: المشاكل الشائعة [وحلولها](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**أواجه مشكلة في إعادة تعيين كلمة مرور المستخدم**

- تأكد من أنك م مخولا لإعادة تعيين كلمات المرور. *يمكن للمسؤولين العامين وكلمة المرور والمستخدمين فقط إعادة تعيين كلمات مرور المستخدمين.* يمكن للمسؤولين العامين أيضا إعادة تعيين كلمات مرور المسؤول المميز الأخرى.

- تأكد من فهم متطلبات الترخيص:

  - يجب أن يكون لديك ترخيص واحد على الأقل تم تعيينه في مؤسستك:
    - **مستخدمو السحابة فقط** - أي Office 365 (O365) مدفوعة من SKU أو Azure AD Basic
    - المستخدمون السحابية **و/أو** المحليون - Azure AD Premium P1 أو P2 أو Enterprise Mobility + Security (EMS) أو Secure Productive Enterprise (SPE)
    - لمعرفة المزيد حول متطلبات الترخيص، راجع متطلبات الترخيص لإعادة تعيين كلمة مرور الخدمة الذاتية ل [Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).
- لإعادة تعيين كلمة مرور المستخدم، ابحث عن المستخدم في Azure AD. بعد ذلك، على شفرة النظرة العامة لهذا المستخدم، انقر فوق الزر "إعادة تعيين كلمة المرور".

**زر إعادة تعيين كلمة المرور رمادي اللون**

أنت غير مصرح لك بإعادة **تعيين** كلمات مرور هذا المستخدم. *يمكن للمسؤولين العامين وكلمة المرور والمستخدمين فقط إعادة تعيين كلمات مرور المستخدمين.* يمكن للمسؤولين العامين أيضا إعادة تعيين كلمات مرور المسؤول المميز الأخرى.

**لا يمكنني رؤية شفرة إعادة تعيين كلمة المرور**

أنت غير مصرح لك بإعادة تعيين كلمات المرور. *يمكن للمسؤولين العامين وكلمة المرور والمستخدمين فقط إعادة تعيين كلمات مرور المستخدمين.* يمكن للمسؤولين العامين أيضا إعادة تعيين كلمات مرور المسؤول المميز الأخرى.

**لا يمكنني رؤية شفرة التكامل المحلي في إعادة تعيين كلمة المرور**

- تظهر ريشة التكامل المحلي فقط في البيئات المختلطة - مما يعني أنك تستخدم إعادة كتابة كلمة المرور لمعالجة كلمات مرور المستخدم المحلي.

- لا ترى هذه الريشة إذا:

  - لا تستخدم إعادة كتابة كلمة المرور
  - توجد مشكلة في تثبيت/اتصال إعادة كتابة كلمة المرور
  - توجد مشكلة في تثبيت/اتصال Azure AD الاتصال
  - لمزيد من خطوات استكشاف الأخطاء وإصلاحها للمشاكل المتعلقة بكتابة كلمة المرور، راجع استكشاف الأخطاء [وإصلاحها في إعادة](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback) كتابة كلمة المرور

**لا أعرف كيفية إعادة تعيين كلمة مرور المستخدم**

1. سجل الدخول إلى مدخل Azure كمسؤول مناسب.
2. انتقل إلى **ريشة المستخدمون والمجموعات،** وحدد **جميع المستخدمين**.
3. حدد مستخدما من القائمة.
4. بالنسبة للمستخدم المحدد، حدد **نظرة عامة**، ثم في شريط الأوامر، حدد إعادة تعيين **كلمة المرور**.
5. حدد الزر **إعادة تعيين كلمة** المرور واتبع الإرشادات الموجودة على الشاشة.
    - لا تدعم عمليات إعادة التعيين التي يتم تنفيذها من خلال **مدخل Azure سوى** إعادة كتابة كلمة المرور.

**أقوم بإعادة تعيين كلمة مرور مستخدم في الموقع Office 365 Admin أو تطبيق Office 365 المحمول ولكن لا يزال المستخدم غير قادر على تسجيل الدخول**

الكتابة بكلمة مرور غير معتمدة في هذا المدخل. أعد تعيين كلمة مرور المستخدم مرة أخرى في مدخل Azure.
