---
title: لا يتم إرسال البريد الإلكتروني لسير العمل
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
ms.openlocfilehash: 2caf8e0878da0049667d9a19f4488eaec4b9327fbf36be7d29dbf4b7a9c89158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072507"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>لا يتم إرسال البريد الإلكتروني لسير العمل لقائمة SharePoint أو مكتبة

1. لا يتم إرسال البريد الإلكتروني من مهام سير العمل إلى كل المستخدمين أو إلى مستخدمين محددين فقط، أو تظهر رسالة الخطأ لا يمكن إرسال رسالة البريد الإلكتروني. تأكد من أن البريد الإلكتروني به **مستلم صالح.**

    تحقق مما إذا كان المستخدم موجودا **في** مجموعة أذونات جميع الأشخاص (قائمة معلومات المستخدم) لمجموعة المواقع هذه.  نموذج عنوان URL المباشر: <tenant> https:// .sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx؟ MembershipGroupId=0

    - إذا لم يكن المستخدم موجودا، فتأكد من تسجيل دخول المستخدم إلى الصفحة. 
    - إذا كان مستخدما خارجيا، فتأكد من قبول دعوته.
    - إذا كان المستخدم موجودا في مجموعة الأذونات، فتأكد من صحة عنوان البريد الإلكتروني.
    - إذا لم يتم تعيين عنوان البريد الإلكتروني للمستخدمين هنا، ف قم بإنشاء تنبيه نموذج لهذا المستخدم الذي يجبر مزامنة حساب المستخدم هذا من ملفات تعريف المستخدمين SharePoint إلى مجموعة المواقع هذه.
 
2. يتم إرسال البريد الإلكتروني من مهام سير العمل إلى مسؤولي مجموعة المواقع المشتركة وليس إلى مستخدمين آخرين وشاهد الخطأ HTTP ممنوع على **<span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    راجع [رفض الوصول عند إرسال رسالة بريد إلكتروني إلى مجموعة](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)SharePoint .

    كذلك، تحقق من **أن** ميزة مجموعة المواقع في وضع تأمين أذونات الوصول المحدود للمستخدم غير نشطة.


## <a name="related-topics"></a>المواضيع ذات الصلة
هل تريد تجربة Microsoft Flow في SharePoint Online؟
- [إنشاء Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


