---
title: مشاكل في تسجيل الدخول إلى التطبيقات
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7788"
- "9004355"
ms.openlocfilehash: 2d073367dc1c3e8e117c0b68e205297a65024872
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900733"
---
# <a name="issues-signing-in-to-applications"></a>مشاكل في تسجيل الدخول إلى التطبيقات

للكشف عن السبب أو تشخيص المشاكل المتعلقة بتسجيل الدخول إلى المستخدم ، قم بتنفيذ الخطوات التالية:

1. شغل [تشخيص تسجيل الدخول](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
2. يمكنك العثور علي الحدث المطلوب تحليله عن طريق إدخال التفاصيل الخاصة بالمستخدم أو التطبيق أو وقت تسجيل الدخول أو معرف الطلب أو معرف الارتباط.
3. راجع نتائج التشخيص التي تعرض تفاصيل حول ما حدث والإجراءات التي يمكنك اتخاذها لاجراء التغييرات ، إذا كانت هناك اي تغييرات مطلوبه.

فيما يلي بعض المشاكل الشائعة التي قد تواجهها عند تسجيل الدخول إلى التطبيقات:

1. لقد قمت أنت أو المستخدم **بإكمال تسجيل الدخول في AZURE AD ، ولكنك تشاهد مطالبه غير متوقعه ،** فراجع المقالات التي تطالب بها [الموافقة الغير متوقعه عند تسجيل الدخول إلى تطبيق](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) [وظهور خطا غير متوقع عند اجراء موافقه علي تطبيق](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).
2. قمت أنت أو المستخدم **بتسجيل الدخول إلى تطبيق مباشره ، ولكن لا يمكنك تسجيل الدخول اليه من ديبلينك علي المدخل المخصص أو علي لوحه الوصول**: راجع [استكشاف الأخطاء وإصلاحها المتعلقة بتسجيل الدخول إلى تطبيق من تطبيقات Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel).
3. قامت أنت أو **المستخدم بإكمال تسجيل الدخول في AZURE AD ، ولكن يعرض التطبيق رسالة خطا ولا يسمح للمستخدم بالانتهاء من تدفق تسجيل الدخول**: المشكلة ان التطبيق لم يقبل الاستجابة التي أصدرها Azure AD. اتبع [هذه الخطوات](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) لاستكشاف الأخطاء وإصلاحها.
4. لا يمكنك أنت أو المستخدم من **تسجيل الدخول إلى تطبيق بدون معرض تم تكوينه لتسجيل الدخول الأحادي إلى كلمه المرور**: اتبع الإرشادات الواردة في [هذه الخطوات](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) لاستكشاف الأخطاء وإصلاحها.
5. لا يمكنك أنت أو المستخدم من **تسجيل الدخول إلى تطبيق معرض AZURE AD الذي تم تكوينه لتسجيل الدخول الأحادي إلى كلمه المرور**: اتبع [الخطوات التالية](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) لاستكشاف الأخطاء وإصلاحها.
6. لا يمكنك أنت أو المستخدم **تسجيل الدخول إلى تطبيق Microsoft**: اتبع [الخطوات التالية](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) لاستكشاف الأخطاء وإصلاحها.
7. لا يمكنك أنت أو المستخدم من **تسجيل الدخول إلى تطبيق بدون معرض تم تكوينه لتسجيل الدخول الأحادي الخارجي**: اتبع [الخطوات التالية](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) لاستكشاف الأخطاء وإصلاحها.
8. لا يمكنك أنت أو المستخدم من **تسجيل الدخول إلى تطبيق معرض AZURE AD تم تكوينه لتسجيل الدخول الأحادي الخارجي**: اتبع [الخطوات التالية](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) لاستكشاف الأخطاء وإصلاحها.
9. لا يمكنك أنت أو المستخدم **تسجيل الدخول إلى تطبيق تم تطويره باستخدام المخصص**: اتبع [الخطوات التالية](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) لاستكشاف الأخطاء وإصلاحها.
10. لا يمكنك أنت أو المستخدم **تسجيل الدخول إلى تطبيق محلي باستخدام وكيل تطبيق AZURE AD**: اتبع [الخطوات التالية](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy) لاستكشاف الأخطاء وإصلاحها.

