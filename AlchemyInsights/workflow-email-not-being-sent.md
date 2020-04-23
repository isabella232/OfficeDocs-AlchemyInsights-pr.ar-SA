---
title: لا يتم إرسال البريد الإلكتروني لسير العمل
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766120"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>لا يتم إرسال البريد الإلكتروني لسير العمل لقائمة SharePoint أو مكتبة

1. لا يتم إرسال البريد الإلكتروني من سير العمل إلى كافة المستخدمين أو مستخدمين محددين فقط، أو ترى الخطأ **لا يمكن إرسال رسالة البريد الإلكتروني. تأكد من أن البريد الإلكتروني يحتوي على مستلم صالح**.

    تحقق مما إذا كان المستخدم موجودًا في مجموعة أذونات **"كافة الأشخاص"** (قائمة معلومات المستخدم) لمجموعة الموقع هذه.  عينة عنوان URL<tenant>المباشر: https:// .sharepoint.com/sites/<sitename>/_layouts/15/people.aspx؟ العضويةGroupId =0

    - إذا لم يكن المستخدم موجوداً، تأكد من تسجيل دخول المستخدم إلى الصفحة. 
    - إذا كان مستخدم ًا خارجيًا، فتأكد من قبول الدعوة الخاصة به.
    - إذا كان المستخدم موجودًا في مجموعة الأذونات، فتأكد من صحة عنوان البريد الإلكتروني.
    - إذا لم يتم تعيين عنوان البريد الإلكتروني للمستخدمين هنا، فقم بإنشاء تنبيه عينة لهذا المستخدم يفرض مزامنة حساب المستخدم هذا من ملفات تعريف المستخدم الخاصة بـ SharePoint إلى مجموعة الموقع هذه.
 
2. يتم إرسال البريد الإلكتروني من سير العمل إلى مسؤولي مجموعة الموقع ولكن ليس إلى مستخدمين آخرين وانظر الخطأ **HTTP ممنوع إلى <span>https:</span>//URL/_vti_bin/client.xvc.sp.utility.utility.SendEmail**.
 

    راجع [رفض الوصول عند إرسال بريد إلكتروني إلى مجموعة SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    أيضاً، تحقق من أن ميزة مجموعة موقع **تأمين إذن المستخدم محدود الوصول** غير نشطة.


## <a name="related-topics"></a>المواضيع ذات الصلة
هل تريد تجربة Microsoft Flow في SharePoint Online؟
- [إنشاء تدفق](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint والتدفق](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


