---
title: لم يتم إرسال البريد الإلكتروني سير العمل
ms.author: efrene
author: efrene
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
ms.openlocfilehash: 261fe1b1bc815dd4ad568051cfefad1e214b957e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530845"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>لم يتم إرسال البريد الإلكتروني سير العمل لقائمة SharePoint أو مكتبته

1. لا يتم إرسال البريد الإلكتروني من مهام سير العمل لكافة المستخدمين أو مستخدمين معينين، أو ترى أنه لا يمكن إرسال خطأ **رسالة البريد الإلكتروني. تأكد من البريد الإلكتروني لمستلم صالح**.

    معرفة ما إذا كان المستخدم موجوداً في مجموعة أذونات **كافة الأشخاص** (قائمة معلومات المستخدم) لمجموعة الموقع هذه.  نموذج عنوان URL مباشرة: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx؟ ميمبيرشيبجروبيد = 0

    - إذا كان المستخدم غير موجود، تأكد من تسجيل المستخدم في الصفحة. 
    - إذا كان مستخدم خارجي، تأكد من أنه تم قبول الدعوة.
    - إذا كان المستخدم موجود في مجموعة أذونات، تأكد من صحة عنوان البريد الإلكتروني.
    - إذا لم يتم تعيين عنوان البريد الإلكتروني المستخدمين هنا، قم بإنشاء تنبيه كعينة لذلك المستخدم الذي يفرض المزامنة لحساب المستخدم هذا من التشكيلات الجانبية للمستخدم من SharePoint إلى مجموعة المواقع المشتركة هذه.
 
2. يتم إرسال لمسؤولي مجموعة الموقع ولكن ليس للمستخدمين الآخرين بالبريد الإلكتروني من مهام سير العمل ومشاهدة الخطأ **HTTP محظور ل <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    راجع [رفض الوصول عند إرسال رسالة بريد إلكتروني لمجموعة SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    تحقق أيضا من ميزة مجموعة موقع **الوصول المحدود إلى وضع تأمين إذن المستخدم** غير نشط.


## <a name="related-topics"></a>المواضيع ذات الصلة
هل ترغب في محاولة تدفق Microsoft SharePoint على الإنترنت؟
- [إنشاء تدفق](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint والتدفق](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


