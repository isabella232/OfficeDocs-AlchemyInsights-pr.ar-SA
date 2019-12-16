---
title: لا يتم إرسال البريد الكتروني سير العمل
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049360"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>لا يتم إرسال البريد الكتروني سير العمل لقائمه أو مكتبه SharePoint

1. لا يتم إرسال البريد الكتروني من مهام سير العمل إلى كافة المستخدمين أو المستخدمين المحددين فقط ، أو تشاهد الخطا **لا يمكن إرسال رسالة البريد الكتروني. تاكد من ان البريد الكتروني يحتوي علي مستلم صالح**.

    تحقق من وجود المستخدم في مجموعه أذونات **الأشخاص كافة** (قائمه معلومات المستخدم) لمجموعه الموقع تلك.  نموذج عنوان URL المباشر<tenant>: https://<sitename>/_layouts/15/sharepoint.com/sites/ العضو المجاميع = 0

    - إذا لم يكن المستخدم موجودا ، تاكد من تسجيل دخول المستخدم إلى الصفحة. 
    - إذا كان مستخدم خارجي ، تاكد من قبول الدعوة الخاصة بهم.
    - إذا كان المستخدم موجودا في مجموعه الأذونات ، تاكد من صحة عنوان البريد الكتروني.
    - إذا لم يتم تعيين عنوان البريد الكتروني للمستخدمين هنا ، قم بإنشاء تنبيه نموذج لهذا المستخدم الذي يفرض مزامنة حساب المستخدم هذا من ملفات تعريف المستخدمين ل SharePoint إلى مجموعه الموقع هذه.
 
2. يتم إرسال البريد الكتروني من مهام سير العمل إلى مسؤولي مجموعه الموقع ولكن ليس إلى المستخدمين الآخرين ومشاهده الخطا **HTTP ممنوع <span>https:</span>//url/_vti_bin/client.xvc.sp.utilities.utility.sendemail**.
 

    راجع [رفض الوصول عند إرسال رسالة بريد الكتروني إلى مجموعه SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    أيضا ، تحقق من ان ميزه مجموعه موقع **تامين اذن المستخدم محدوده الوصول** غير نشطه.


## <a name="related-topics"></a>المواضيع ذات الصلة
هل تريد محاولة Microsoft Flow في SharePoint علي الإنترنت ؟
- [إنشاء تدفق](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint والتدفق](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


