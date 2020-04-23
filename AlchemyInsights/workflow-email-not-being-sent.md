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
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="87d0b-102">لا يتم إرسال البريد الإلكتروني لسير العمل لقائمة SharePoint أو مكتبة</span><span class="sxs-lookup"><span data-stu-id="87d0b-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="87d0b-103">لا يتم إرسال البريد الإلكتروني من سير العمل إلى كافة المستخدمين أو مستخدمين محددين فقط، أو ترى الخطأ **لا يمكن إرسال رسالة البريد الإلكتروني. تأكد من أن البريد الإلكتروني يحتوي على مستلم صالح**.</span><span class="sxs-lookup"><span data-stu-id="87d0b-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="87d0b-104">تحقق مما إذا كان المستخدم موجودًا في مجموعة أذونات **"كافة الأشخاص"** (قائمة معلومات المستخدم) لمجموعة الموقع هذه.</span><span class="sxs-lookup"><span data-stu-id="87d0b-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="87d0b-105">عينة عنوان URL<tenant>المباشر: https:// .sharepoint.com/sites/<sitename>/_layouts/15/people.aspx؟ العضويةGroupId =0</span><span class="sxs-lookup"><span data-stu-id="87d0b-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="87d0b-106">إذا لم يكن المستخدم موجوداً، تأكد من تسجيل دخول المستخدم إلى الصفحة.</span><span class="sxs-lookup"><span data-stu-id="87d0b-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="87d0b-107">إذا كان مستخدم ًا خارجيًا، فتأكد من قبول الدعوة الخاصة به.</span><span class="sxs-lookup"><span data-stu-id="87d0b-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="87d0b-108">إذا كان المستخدم موجودًا في مجموعة الأذونات، فتأكد من صحة عنوان البريد الإلكتروني.</span><span class="sxs-lookup"><span data-stu-id="87d0b-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="87d0b-109">إذا لم يتم تعيين عنوان البريد الإلكتروني للمستخدمين هنا، فقم بإنشاء تنبيه عينة لهذا المستخدم يفرض مزامنة حساب المستخدم هذا من ملفات تعريف المستخدم الخاصة بـ SharePoint إلى مجموعة الموقع هذه.</span><span class="sxs-lookup"><span data-stu-id="87d0b-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="87d0b-110">يتم إرسال البريد الإلكتروني من سير العمل إلى مسؤولي مجموعة الموقع ولكن ليس إلى مستخدمين آخرين وانظر الخطأ **HTTP ممنوع إلى <span>https:</span>//URL/_vti_bin/client.xvc.sp.utility.utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="87d0b-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="87d0b-111">راجع [رفض الوصول عند إرسال بريد إلكتروني إلى مجموعة SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="87d0b-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="87d0b-112">أيضاً، تحقق من أن ميزة مجموعة موقع **تأمين إذن المستخدم محدود الوصول** غير نشطة.</span><span class="sxs-lookup"><span data-stu-id="87d0b-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="87d0b-113">المواضيع ذات الصلة</span><span class="sxs-lookup"><span data-stu-id="87d0b-113">Related topics</span></span>
<span data-ttu-id="87d0b-114">هل تريد تجربة Microsoft Flow في SharePoint Online؟</span><span class="sxs-lookup"><span data-stu-id="87d0b-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="87d0b-115">إنشاء تدفق</span><span class="sxs-lookup"><span data-stu-id="87d0b-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="87d0b-116">SharePoint والتدفق</span><span class="sxs-lookup"><span data-stu-id="87d0b-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


