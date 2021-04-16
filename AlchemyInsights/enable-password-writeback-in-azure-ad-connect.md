---
title: تمكين الكتابة بكلمة مرور في Azure AD Connect
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 2ad7568bded3c8e4832e0e433a2d715e6307e4bb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813999"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>تمكين الكتابة بكلمة مرور في Azure AD Connect

لتمكين إعادة تعيين الكتابة بكلمة مرور الخدمة الذاتية، قم أولا بتمكين خيار الكتابة في Azure AD Connect. من خادم Azure AD Connect، أكمل الخطوات التالية:

1. سجل الدخول إلى خادم Azure AD Connect وابدأ معالج تكوين **Azure AD Connect.**
2. في صفحة **الترحيب،** انقر فوق **تكوين**.
3. في صفحة **المهام الإضافية،** حدد **تخصيص خيارات المزامنة**، ثم انقر فوق **التالي**.
4. في صفحة **الاتصال ب Azure AD،** أدخل بيانات اعتماد المسؤول العام لمستأجر Azure، ثم انقر فوق **التالي**.
5. في **صفحتي تصفية** الدلائل و **Domain/OU** Connect، انقر فوق **التالي**.
6. في صفحة **الميزات الاختيارية،** حدد المربع بجانب إعادة كتابة كلمة **المرور** وانقر فوق **التالي**.
7. في الصفحة **جاهز للتكوين،** انقر فوق **تكوين** وانتظر حتى تنتهي العملية.
8. عندما ترى انتهاء التكوين، انقر فوق **إنهاء**.

مع تمكين إعادة كتابة كلمة المرور في Azure AD Connect، قم بتكوين Azure AD SSPR للكتابة.  لتمكين كتابة كلمة المرور في SSPR، أكمل الخطوات التالية:

1. سجل الدخول إلى مدخل Azure باستخدام حساب مسؤول عام.
2. ابحث عن **Azure Active Directory** وحدده، وانقر **فوق** إعادة تعيين كلمة المرور، ثم انقر فوق **التكامل المحلي.**
3. هل تريد تعيين الخيار **"إعادة كتابة كلمات المرور"** إلى الدليل الخاص بك في الموقع؟ إلى **نعم.**
4. قم بتعيين الخيار السماح **للمستخدمين بإلغاء تأمين الحسابات دون إعادة تعيين كلمة المرور الخاصة بهم؟** إلى **نعم.**
5. عندما تكون جاهزا، انقر فوق **حفظ**.

لمزيد من المعلومات، راجع تمكين إعادة تعيين كلمة مرور الخدمة الذاتية [ل Azure Active Directory إلى بيئة المحلية](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).

> [!NOTE]
>  عندما يقوم مسؤول بإعادة تعيين كلمة مرور مستخدم في مدخل Azure، إذا كان هذا المستخدم موحا أو متزامنا مع كلمة المرور، يتم إعادة كتابة كلمة المرور إلى الموقع. تتطلب هذه الوظيفة ترخيص Azure Premium (P1 أو P2) وهو غير معتمد حاليا في مدخل مسؤول Office.
