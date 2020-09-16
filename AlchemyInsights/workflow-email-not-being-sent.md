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
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="3aa68-102">لم يتم إرسال البريد الكتروني لسير العمل لقائمه أو مكتبه SharePoint</span><span class="sxs-lookup"><span data-stu-id="3aa68-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="3aa68-103">لا يتم إرسال البريد الكتروني من مهام سير العمل إلى جميع المستخدمين أو المستخدمين المحددين فقط ، أو يظهر الخطا **تعذر إرسال رسالة البريد الكتروني. تاكد من ان البريد الكتروني يملك مستلما صالحا**.</span><span class="sxs-lookup"><span data-stu-id="3aa68-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="3aa68-104">تحقق مما إذا كان المستخدم موجودا في مجموعه أذونات **جميع الأشخاص** (معلومات المستخدم) لمجموعه المواقع المشتركة تلك.</span><span class="sxs-lookup"><span data-stu-id="3aa68-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="3aa68-105">نموذج URL مباشر: https:// <tenant> /sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx ؟ ميمبيرشيبجروبيد = 0</span><span class="sxs-lookup"><span data-stu-id="3aa68-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="3aa68-106">إذا لم يكن المستخدم موجودا ، فتاكد من ان المستخدم قد قام بتسجيل الدخول إلى الصفحة.</span><span class="sxs-lookup"><span data-stu-id="3aa68-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="3aa68-107">إذا كان أحد المستخدمين الخارجيين ، فتاكد من قبول دعوتهم.</span><span class="sxs-lookup"><span data-stu-id="3aa68-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="3aa68-108">إذا كان المستخدم موجودا في المجموعة الأذونات ، فتاكد من صحة عنوان البريد الكتروني.</span><span class="sxs-lookup"><span data-stu-id="3aa68-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="3aa68-109">إذا لم يتم تعيين عنوان البريد الكتروني للمستخدمين هنا ، فقم بإنشاء تنبيه نموذجي لذلك المستخدم الذي يفرض مزامنة حساب المستخدم هذا من ملفات تعريف المستخدمين في SharePoint إلى مجموعه المواقع المشتركة هذه.</span><span class="sxs-lookup"><span data-stu-id="3aa68-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="3aa68-110">يتم إرسال البريد الكتروني من مهام سير العمل إلى مسؤولي مجموعه المواقع المشتركة وليس إلى المستخدمين الآخرين وراجع الخطا **HTTP حظر إلى <span>https:</span>//url/_vti_bin/client.xvc.sp.utilities.utility.sendemail**.</span><span class="sxs-lookup"><span data-stu-id="3aa68-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="3aa68-111">راجع [رفض الوصول عند إرسال رسالة بريد الكتروني إلى مجموعه SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="3aa68-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="3aa68-112">تاكد أيضا من عدم تنشيط ميزه مجموعه المواقع المشتركة **لوضع تامين الأذونات الخاصة بالمستخدم** .</span><span class="sxs-lookup"><span data-stu-id="3aa68-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="3aa68-113">المواضيع ذات الصلة</span><span class="sxs-lookup"><span data-stu-id="3aa68-113">Related topics</span></span>
<span data-ttu-id="3aa68-114">هل تريد تجربه Microsoft تدفق في SharePoint Online ؟</span><span class="sxs-lookup"><span data-stu-id="3aa68-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="3aa68-115">إنشاء تدفق</span><span class="sxs-lookup"><span data-stu-id="3aa68-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="3aa68-116">SharePoint والتدفق</span><span class="sxs-lookup"><span data-stu-id="3aa68-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


