---
title: لم يتم إرسال البريد الكتروني لسير العمل
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748976"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>لم يتم إرسال البريد الكتروني لسير العمل لقائمه أو مكتبه SharePoint

1. لا يتم إرسال البريد الكتروني من مهام سير العمل إلى جميع المستخدمين أو المستخدمين المحددين فقط ، أو يظهر الخطا **تعذر إرسال رسالة البريد الكتروني. تاكد من ان البريد الكتروني يملك مستلما صالحا**.

    تحقق مما إذا كان المستخدم موجودا في مجموعه أذونات **جميع الأشخاص** (معلومات المستخدم) لمجموعه المواقع المشتركة تلك.  نموذج URL مباشر: https:// <tenant> /sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx ؟ ميمبيرشيبجروبيد = 0

    - إذا لم يكن المستخدم موجودا ، فتاكد من ان المستخدم قد قام بتسجيل الدخول إلى الصفحة. 
    - إذا كان أحد المستخدمين الخارجيين ، فتاكد من قبول دعوتهم.
    - إذا كان المستخدم موجودا في المجموعة الأذونات ، فتاكد من صحة عنوان البريد الكتروني.
    - إذا لم يتم تعيين عنوان البريد الكتروني للمستخدمين هنا ، فقم بإنشاء تنبيه نموذجي لذلك المستخدم الذي يفرض مزامنة حساب المستخدم هذا من ملفات تعريف المستخدمين في SharePoint إلى مجموعه المواقع المشتركة هذه.
 
2. يتم إرسال البريد الكتروني من مهام سير العمل إلى مسؤولي مجموعه المواقع المشتركة وليس إلى المستخدمين الآخرين وراجع الخطا **HTTP حظر إلى <span>https:</span>//url/_vti_bin/client.xvc.sp.utilities.utility.sendemail**.
 

    راجع [رفض الوصول عند إرسال رسالة بريد الكتروني إلى مجموعه SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    تاكد أيضا من عدم تنشيط ميزه مجموعه المواقع المشتركة **لوضع تامين الأذونات الخاصة بالمستخدم** .


## <a name="related-topics"></a>المواضيع ذات الصلة
هل تريد تجربه Microsoft تدفق في SharePoint Online ؟
- [إنشاء تدفق](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint والتدفق](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


