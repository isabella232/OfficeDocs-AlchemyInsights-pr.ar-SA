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
ms.openlocfilehash: 49c510668f4c73a71495b89ee9f810d4e7244da3
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270659"
---
# <a name="workflow-email-is-not-being-sent"></a>لم يتم إرسال البريد الإلكتروني سير العمل

1. لا يتم إرسال البريد الإلكتروني من مهام سير العمل لكافة المستخدمين أو مستخدمين معينين، أو ترى أنه لا يمكن إرسال خطأ **رسالة البريد الإلكتروني. تأكد من البريد الإلكتروني لمستلم صالح**.

    معرفة ما إذا كان المستخدم موجوداً في مجموعة أذونات **كافة الأشخاص** (قائمة معلومات المستخدم) لمجموعة الموقع هذه.  نموذج عنوان URL مباشرة: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx؟ ميمبيرشيبجروبيد = 0

    - إذا كان المستخدم غير موجود، تأكد من تسجيل المستخدم في الصفحة. 
    - إذا كان مستخدم خارجي، تأكد من أنه تم قبول الدعوة.
    - إذا كان المستخدم موجود في مجموعة أذونات، تأكد من صحة عنوان البريد الإلكتروني.
    - إذا لم يتم تعيين عنوان البريد الإلكتروني المستخدمين هنا، قم بإنشاء تنبيه كعينة لذلك المستخدم الذي يفرض المزامنة لحساب المستخدم هذا من التشكيلات الجانبية للمستخدم من SharePoint إلى مجموعة المواقع المشتركة هذه.
 
2. يتم إرسال لمسؤولي مجموعة الموقع ولكن ليس للمستخدمين الآخرين بالبريد الإلكتروني من مهام سير العمل ومشاهدة الخطأ **HTTP محظور ل <spam> <spam> ** <spam> <spam>.
 

    راجع [رفض الوصول عند تجميع رسائل البريد الإلكتروني المرسلة إلى](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).

    تحقق أيضا من ميزة مجموعة موقع **الوصول المحدود إلى وضع تأمين إذن المستخدم** غير نشط.


## <a name="related-topics"></a>المواضيع ذات الصلة
هل ترغب في محاولة تدفق Microsoft SharePoint على الإنترنت؟
- [إنشاء تدفق](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint والتدفق](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


