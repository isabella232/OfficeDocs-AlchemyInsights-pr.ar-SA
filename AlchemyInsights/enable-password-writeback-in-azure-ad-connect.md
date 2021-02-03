---
title: تمكين إعادة كتابة كلمة المرور في Azure AD Connect
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 1e90aedab20c8abaa021ed980e868cea0503b7b1
ms.sourcegitcommit: db95fd628c45d9810e5af5c5a4e6388c793339ac
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093342"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>تمكين إعادة كتابة كلمة المرور في Azure AD Connect

لتمكين إعادة تعيين الكتابة بكلمة مرور الخدمة الذاتية، قم أولا بتمكين خيار الكتابة في Azure AD Connect. من خادم Azure AD Connect، أكمل الخطوات التالية:

1. سجل الدخول إلى خادم Azure AD Connect وابدأ معالج تكوين **Azure AD Connect.**
2. على صفحة **الترحيب،** انقر فوق **"تكوين".**
3. في صفحة **المهام الإضافية،** حدد **"تخصيص خيارات المزامنة"،** ثم انقر فوق **"التالي".**
4. في صفحة **"الاتصال ب Azure AD"،** أدخل بيانات اعتماد المسؤول العام لمستأجر Azure، ثم انقر فوق **"التالي".**
5. في صفحات تصفية الدلائل **والمجال/OU** في Connect، انقر فوق **"التالي".** 
6. في صفحة **الميزات الاختيارية،** حدد المربع بجانب إعادة كتابة كلمة **المرور** وانقر فوق **"التالي".**
7. في الصفحة **"جاهز لتكوين"،** انقر فوق **"تكوين"** وانتظر حتى تنتهي العملية.
8. عندما ترى انتهاء التكوين، انقر فوق **"إنهاء".**

مع تمكين إعادة كتابة كلمة المرور في Azure AD Connect، قم بتكوين Azure AD SSPR للكتابة.  لتمكين إعادة كتابة كلمة المرور في SSPR، أكمل الخطوات التالية:

1. سجل الدخول إلى مدخل Azure باستخدام حساب مسؤول عام.
2. ابحث عن **Azure Active Directory** وحدده، وانقر فوق إعادة **تعيين** كلمة المرور، ثم انقر **فوق التكامل المحلي.**
3. تعيين خيار إعادة كتابة كلمات المرور إلى الدليل **في الموقع؟** إلى **"نعم".**
4. تعيين الخيار "السماح للمستخدمين بإلغاء تأمين الحسابات دون إعادة تعيين كلمة المرور **الخاصة بهم"؟** إلى **"نعم".**
5. عندما تكون جاهزا، انقر فوق **"حفظ".**

لمزيد من المعلومات، راجع ["تمكين خدمة Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback)الذاتية" لإعادة تعيين إعادة الكتابة إلى بيئة المحلية.

> [!NOTE]
>  عندما يعيد المسؤول تعيين كلمة مرور مستخدم في مدخل Azure، إذا كان هذا المستخدم موحنا أو متزامنا مع كلمة المرور، يتم إعادة كتابة كلمة المرور إلى الموقع تتطلب هذه الوظيفة ترخيص Azure Premium (P1 أو P2) وهو غير معتمد حاليا في مدخل مسؤول Office.
