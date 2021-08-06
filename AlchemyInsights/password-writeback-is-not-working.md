---
title: لا يعمل "الكتابة بكلمة مرور"
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
- "9004595"
- "8210"
ms.openlocfilehash: 23f5e5fe9e00a4bb00f96d2023c81f6413a7d8b808fd46bfc94483944bb898dc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999731"
---
# <a name="password-writeback-is-not-working"></a>لا يعمل "الكتابة بكلمة مرور"

**أواجه مشاكل في تكوين إعادة كتابة كلمة المرور**

- الكتابة بكلمة مرور هي ميزة متميزة.
- تأكد من فهم متطلبات الترخيص:
  - يجب أن يكون لديك ترخيص واحد على الأقل تم تعيينه في مؤسستك
  - **مستخدمو السحابة فقط** - أي Office 365 (O365) مدفوعة من SKU أو Azure AD Basic
  - المستخدمون السحابية **و/أو** المحليون - Azure AD Premium P1 أو P2 أو Enterprise Mobility + Security (EMS) أو Secure Productive Enterprise (SPE)
    - لمعرفة المزيد حول متطلبات الترخيص، راجع متطلبات الترخيص لإعادة تعيين كلمة مرور الخدمة الذاتية ل [Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- لديك حساب مسؤول واحد على الأقل حساب مستخدم اختباري واحد مع أحد الترخيص المناسب.
- يجب توصيل Azure AD الاتصال "محاكي وحدة التحكم بالمجال الأساسي" لكي تعمل إعادة كتابة كلمة المرور. يمكنك تكوين Azure AD الاتصال لاستخدام وحدة تحكم المجال الأساسية بالنقر  بيمين فوق خصائص موصل مزامنة Active Directory، ثم تحديد تكوين **أقسام الدليل**. من هناك، ابحث عن المقطع **إعدادات** اتصال وحدة التحكم بالمجال ودقق في المربع الذي يحمل العنوان استخدام وحدات تحكم المجال **المفضلة فقط.**
  > [!NOTE]
  > إذا لم تكن DC المفضلة من محاكي PDC، فإن Azure AD الاتصال يزال يصل إلى PDC للكتابة بكلمة مرور.
- تم تكوين إعادة تعيين كلمة المرور وتمكينها في المستأجر. لمزيد من المعلومات، راجع تمكين المستخدمين من إعادة تعيين كلمات مرور [Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)الخاصة بهم .
- تأكد من أن حساب المسؤول الذي يتم استخدامه لتمكين "كتابة كلمة المرور" هو حساب مسؤول السحابة (تم إنشاؤه في Azure AD وليس AD المحلي)
- لديك نشر AD في موقع واحد أو متعدد الغابات يعمل على Windows Server 2008 R2 أو Windows Server 2012 أو Windows Server 2012 R2 مع تثبيت أحدث حزم الخدمة
- تم تثبيت أداة Azure AD الاتصال وقد أعددت بيئة AD للمزامنة مع السحابة. قبل اختبار إعادة كتابة كلمة المرور، تأكد من إكمال عملية الاستيراد والمزامنة الكاملة أولا من كل من AD و Azure AD في Azure AD الاتصال.
- لمعرفة المزيد، راجع كيفية القيام بالمزامنة الكاملة [والاستيراد الكامل في Azure AD الاتصال](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**أواجه مشكلة في اتصال الكتابة بكلمة مرور**

1. تنزيل أحدث إصدار من [Azure AD](https://www.microsoft.com/download/details.aspx?id=47594) الاتصال
2. تكوين جدار الحماية: ستحتاج أداة Azure AD الاتصال (1.1.443 والأعلى) إلى الوصول **إلى HTTPS** الصادر إلى:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. السماح لاتصالات الخمول أن تستمر لمدة 2-3 دقائق على الأقل

**ما زلت أواجه مشاكل في كتابة كلمة المرور**

- إذا كنت لا تزال تواجه صعوبة، فحاول تعطيل خدمة الكتابة بكلمة مرور في أداة Azure AD الاتصال إعادة تمكينها
- لمعرفة المزيد، راجع كيفية تعطيل إعادة تمكين إعادة كتابة كلمة [المرور](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
