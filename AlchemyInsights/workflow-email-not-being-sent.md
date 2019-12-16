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
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="12c39-102">لا يتم إرسال البريد الكتروني سير العمل لقائمه أو مكتبه SharePoint</span><span class="sxs-lookup"><span data-stu-id="12c39-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="12c39-103">لا يتم إرسال البريد الكتروني من مهام سير العمل إلى كافة المستخدمين أو المستخدمين المحددين فقط ، أو تشاهد الخطا **لا يمكن إرسال رسالة البريد الكتروني. تاكد من ان البريد الكتروني يحتوي علي مستلم صالح**.</span><span class="sxs-lookup"><span data-stu-id="12c39-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="12c39-104">تحقق من وجود المستخدم في مجموعه أذونات **الأشخاص كافة** (قائمه معلومات المستخدم) لمجموعه الموقع تلك.</span><span class="sxs-lookup"><span data-stu-id="12c39-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="12c39-105">نموذج عنوان URL المباشر<tenant>: https://<sitename>/_layouts/15/sharepoint.com/sites/ العضو المجاميع = 0</span><span class="sxs-lookup"><span data-stu-id="12c39-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="12c39-106">إذا لم يكن المستخدم موجودا ، تاكد من تسجيل دخول المستخدم إلى الصفحة.</span><span class="sxs-lookup"><span data-stu-id="12c39-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="12c39-107">إذا كان مستخدم خارجي ، تاكد من قبول الدعوة الخاصة بهم.</span><span class="sxs-lookup"><span data-stu-id="12c39-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="12c39-108">إذا كان المستخدم موجودا في مجموعه الأذونات ، تاكد من صحة عنوان البريد الكتروني.</span><span class="sxs-lookup"><span data-stu-id="12c39-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="12c39-109">إذا لم يتم تعيين عنوان البريد الكتروني للمستخدمين هنا ، قم بإنشاء تنبيه نموذج لهذا المستخدم الذي يفرض مزامنة حساب المستخدم هذا من ملفات تعريف المستخدمين ل SharePoint إلى مجموعه الموقع هذه.</span><span class="sxs-lookup"><span data-stu-id="12c39-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="12c39-110">يتم إرسال البريد الكتروني من مهام سير العمل إلى مسؤولي مجموعه الموقع ولكن ليس إلى المستخدمين الآخرين ومشاهده الخطا **HTTP ممنوع <span>https:</span>//url/_vti_bin/client.xvc.sp.utilities.utility.sendemail**.</span><span class="sxs-lookup"><span data-stu-id="12c39-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="12c39-111">راجع [رفض الوصول عند إرسال رسالة بريد الكتروني إلى مجموعه SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="12c39-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="12c39-112">أيضا ، تحقق من ان ميزه مجموعه موقع **تامين اذن المستخدم محدوده الوصول** غير نشطه.</span><span class="sxs-lookup"><span data-stu-id="12c39-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="12c39-113">المواضيع ذات الصلة</span><span class="sxs-lookup"><span data-stu-id="12c39-113">Related topics</span></span>
<span data-ttu-id="12c39-114">هل تريد محاولة Microsoft Flow في SharePoint علي الإنترنت ؟</span><span class="sxs-lookup"><span data-stu-id="12c39-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="12c39-115">إنشاء تدفق</span><span class="sxs-lookup"><span data-stu-id="12c39-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="12c39-116">SharePoint والتدفق</span><span class="sxs-lookup"><span data-stu-id="12c39-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


