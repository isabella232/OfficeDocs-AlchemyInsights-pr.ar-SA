---
title: لا يعمل "كتابة كلمة المرور"
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
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243217"
---
# <a name="password-writeback-is-not-working"></a>لا يعمل "كتابة كلمة المرور"

**أواجه مشاكل في تكوين إعادة كتابة كلمة المرور**

- الكتابة بكلمة مرور هي ميزة متميزة.
- تأكد من فهم متطلبات الترخيص:
  - يجب أن يكون لديك ترخيص واحد على الأقل تم تعيينه في مؤسستك
  - **مستخدمو السحابة فقط** - أي SKU مدفوعة من Office 365 (O365) أو Azure AD Basic
  - المستخدمون في السحابة **و/أو** المحليون - Azure AD Premium P1 أو P2 أو Enterprise Mobility + Security (EMS) أو Secure Productive Enterprise (SPE)
    - لمعرفة المزيد حول متطلبات الترخيص، راجع متطلبات الترخيص لإعادة تعيين كلمة مرور الخدمة الذاتية ل [Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- لديك حساب مسؤول واحد على الأقل، حساب مستخدم اختباري واحد مع أحد الترخيص المناسب.
- يجب توصيل Azure AD Connect ب "محاكي وحدة تحكم المجال الأساسية" لكي تعمل كتابة كلمة المرور. يمكنك تكوين Azure AD Connect لاستخدام وحدة التحكم بالمجال  الأساسي بالنقر ب الماوس الأيمن فوق خصائص موصل مزامنة Active Directory، ثم تحديد أقسام تكوين **الدليل.** من هناك، ابحث  عن مقطع إعدادات اتصال وحدة التحكم بالمجال ودقق في المربع بعنوان استخدام وحدات تحكم المجال **المفضلة فقط.**
  > [!NOTE]
  > إذا لم تكن DC المفضلة محاكاة PDC، فإن Azure AD Connect سيبقى يصل إلى PDC لكتابة كلمة المرور.
- تم تكوين إعادة تعيين كلمة المرور وتمكينها في المستأجر. لمزيد من المعلومات، راجع ["تمكين المستخدمين" من إعادة تعيين كلمات مرور Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- تأكد من أن حساب المسؤول الذي يتم استخدامه لتمكين "كتابة كلمة المرور" هو حساب مسؤول مجموعة النظراء (تم إنشاؤه في Azure AD وليس AD المحلي)
- لديك نشر AD واحد أو متعدد الغابات في موقع ويب يعمل بنظام التشغيل Windows Server 2008 R2 أو Windows Server 2012 أو Windows Server 2012 R2 مع تثبيت أحدث حزم الخدمات
- لديك أداة Azure AD Connect مثبتة وقد أعددت بيئة AD للمزامنة إلى السحابة. قبل اختبار إعادة كتابة كلمة المرور، تأكد من إكمال عملية الاستيراد والمزامنة الكاملة أولا من كل من AD و Azure AD في Azure AD Connect.
- لمعرفة المزيد، راجع كيفية القيام بمزامنة [واستيراد كامل في Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**أواجه مشكلة في اتصال إعادة كتابة كلمة المرور**

1. تنزيل أحدث إصدار من [Azure AD Connect وتمكينه](https://www.microsoft.com/download/details.aspx?id=47594)
2. تكوين جدار الحماية: ستحتاج أداة Azure AD Connect (1.1.443 والأعلى) إلى الوصول الصادر **إلى HTTPS:**
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. السماح لاتصالات الخمول أن تستمر لمدة 2-3 دقائق على الأقل

**ما زلت أواجه مشاكل في إعادة كتابة كلمة المرور**

- إذا كنت لا تزال تواجه صعوبة، فحاول تعطيل خدمة إعادة كتابة كلمة المرور في أداة Azure AD Connect ثم إعادة تمكينها
- لمعرفة المزيد، راجع كيفية [تعطيل إعادة تمكين إعادة كتابة كلمة المرور](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
