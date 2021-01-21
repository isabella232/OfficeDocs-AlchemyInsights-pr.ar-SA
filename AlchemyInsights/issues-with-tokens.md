---
title: مشاكل تتعلق بالرموز المميزة
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7774"
- "9004351"
ms.openlocfilehash: 14a9681c08920094813497e7a75eb87bb0733cbc
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/20/2021
ms.locfileid: "49916656"
---
# <a name="issues-with-tokens"></a>مشاكل تتعلق بالرموز المميزة

لأداره المشاكل المتعلقة بالرموز المميزة ، يمكنك تنفيذ الخطوات التالية:

1. يمكنك تحديد مده بقاء الوصول أو المعرف أو الرمز المميز لSAML الذي تم إصداره بواسطة النظام الأساسي لهويه Microsoft. يمكنك تعيين اعمار الرموز المميزة لجميع التطبيقات في مؤسستك ، للحصول علي تطبيق متعدد المستاجرين (متعدد المؤسسات) ، أو لحساب خدمه معين في مؤسستك. للحصول علي مزيد من المعلومات ، راجع فترات [بقاء الرمز القابل للتكوين في Microsoft identity platform (معاينه)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
2. تمكن الرموز المميزة في Access العملاء من الاتصال بأمان واجات برمجه تطبيقات ويب المحمية بشكل أمن ، ويتم استخدامها بواسطة واجات برمجه تطبيقات ويب لتنفيذ المصادقة والتخويل وفقا لمواصفات OAuth ، تكون الرموز المميزة للوصول سلاسل غير واضحة بدون تنسيق المجموعة-يتم استخدام معرفات المستخدمين لبعض موفري الهويات (إيدبس) في ثنائي. يستخدم النظام الأساسي لهويه Microsoft مجموعه متنوعة من تنسيقات الرمز المميز للوصول ، استنادا إلى تكوين واجهه برمجه التطبيق (API) التي تقبل الرمز المميز. للتعرف علي كيفيه تمكن واجهه برمجه التطبيق (API) من التحقق من صحة المطالبات داخل رمز مميز للوصول واستخدامها ، راجع [رموز الوصول للنظام الأساسي لهويه Microsoft](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint).
3. تدعم مكتبه المصادقة من Microsoft (مسال) تدفقات المصادقة المتعددة لاستخدامها في سيناريوهات تطبيقات مختلفه. لمزيد من المعلومات ، راجع [تدفقات المصادقة](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes).
4. يمكن استخدام منح الكود OAuth 2.0 في التطبيقات المثبتة علي جهاز للحصول علي حق الوصول إلى الموارد المحمية ، مثل واجات برمجه تطبيقات ويب. باستخدام تطبيق Microsoft identity platform ل OAuth 2.0 ، يمكنك أضافه امكانيه الوصول إلى تطبيقات الاجهزه المحمولة وبرامج سطح المكتب في windows. راجع [النظام الأساسي لهويه Microsoft و OAuth 2.0 تدفق التعليمات البرمجية](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token) للتعرف علي كيفيه البرمجة مباشره مقابل البروتوكول في التطبيق ، باستخدام اي لغة.
5. أوبينيد Connect (أويدك) بروتوكول مصادقه تم إنشاؤه علي OAuth 2.0 الذي يمكنك استخدامه لتسجيل الدخول بأمان إلى تطبيق ما. عند استخدام تطبيق نقطه نهاية Microsoft identity platform ل أوبينيد Connect ، يمكنك أضافه تسجيل الدخول والوصول إلى API إلى تطبيقاتك. يظهر [النظام الأساسي لهويه Microsoft وبروتوكول اتصال أوبينيد](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request) الآن كيفيه تنفيذ هذا الاجراء بشكل مستقل عن اللغة ويصف كيفيه إرسال رسائل HTTP وتلقيها بدون استخدام اي من مكتبات المصادر المفتوحة من Microsoft.
    - أوسيرينفو نقطه النهاية الخاصة بالمستخدم جزءا من الأويدك القياسية ، والمصممة لإرجاع المطالبات التي تمت المصادقة عليها. للحصول علي مزيد من المعلومات ، راجع [نقطه نهاية أوسيرينفو النظام الأساسي لهويه Microsoft](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead).
    - يبين [الاتصال بواجهة برمجه تطبيقات ويب في تطبيق ويب باستخدام نموذج الاتصال الخاص ب AZURE ad And أوبينيد](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) كيفيه إنشاء تطبيق ويب ل MVC يستخدم azure ad لتسجيل الدخول باستخدام بروتوكول أوبينيد Connect ، ثم الاتصال بواجهة برمجه تطبيقات ويب ضمن هويه المستخدم الذي تم تسجيل دخوله باستخدام الرموز المميزة التي تم الحصول عليها عبر OAuth 2.0. يستخدم هذا النموذج الوسيطة أوبينيد الخاصة ب ASP .Net عون
6. [تكوين تطبيق لعرض واجهه برمجه التطبيقات علي ويب](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis) -في هذا التشغيل ، يمكنك تسجيل واجهه برمجه تطبيقات ويب بواسطة النظام الأساسي لهويه Microsoft وعرضها إلى تطبيقات العميل عبر أضافه نطاق مثال. من خلال تسجيل واجهه برمجه التطبيقات علي ويب وعرضها عبر النطاقات ، يمكنك توفير امكانيه الوصول المستند إلى الأذونات إلى مواردها إلى المستخدمين المخولين وتطبيقات العميل التي تصل إلى واجهه برمجه التطبيقات الخاصة بك.
7. في Azure Active directory B2C (Azure AD B2C) ، تكون بيانات اعتماد مالك الموارد (روبك) تدفق المصادقة القياسية OAuth. في هذا التدفق ، يقوم تطبيق ، والمعروف أيضا بجهة الاعتماد ، بتبادل بيانات الاعتماد الصالحة للرموز المميزة. تتضمن بيانات الاعتماد معرف مستخدم وكلمه مرور. الرموز المميزة التي يتم إرجاعها عبارة عن رمز مميز لمعرف ، ورمز الوصول ، ورمز تحديث مميز. لمزيد من المعلومات ، راجع اعداد [تدفق بيانات اعتماد مالك الموارد في Azure Active DIRECTORY B2C](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow). 

