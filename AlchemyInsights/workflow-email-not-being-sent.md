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
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="a89bc-102">لم يتم إرسال البريد الإلكتروني سير العمل لقائمة SharePoint أو مكتبته</span><span class="sxs-lookup"><span data-stu-id="a89bc-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="a89bc-103">لا يتم إرسال البريد الإلكتروني من مهام سير العمل لكافة المستخدمين أو مستخدمين معينين، أو ترى أنه لا يمكن إرسال خطأ **رسالة البريد الإلكتروني. تأكد من البريد الإلكتروني لمستلم صالح**.</span><span class="sxs-lookup"><span data-stu-id="a89bc-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="a89bc-104">معرفة ما إذا كان المستخدم موجوداً في مجموعة أذونات **كافة الأشخاص** (قائمة معلومات المستخدم) لمجموعة الموقع هذه.</span><span class="sxs-lookup"><span data-stu-id="a89bc-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="a89bc-105">نموذج عنوان URL مباشرة: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx؟ ميمبيرشيبجروبيد = 0</span><span class="sxs-lookup"><span data-stu-id="a89bc-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="a89bc-106">إذا كان المستخدم غير موجود، تأكد من تسجيل المستخدم في الصفحة.</span><span class="sxs-lookup"><span data-stu-id="a89bc-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="a89bc-107">إذا كان مستخدم خارجي، تأكد من أنه تم قبول الدعوة.</span><span class="sxs-lookup"><span data-stu-id="a89bc-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="a89bc-108">إذا كان المستخدم موجود في مجموعة أذونات، تأكد من صحة عنوان البريد الإلكتروني.</span><span class="sxs-lookup"><span data-stu-id="a89bc-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="a89bc-109">إذا لم يتم تعيين عنوان البريد الإلكتروني المستخدمين هنا، قم بإنشاء تنبيه كعينة لذلك المستخدم الذي يفرض المزامنة لحساب المستخدم هذا من التشكيلات الجانبية للمستخدم من SharePoint إلى مجموعة المواقع المشتركة هذه.</span><span class="sxs-lookup"><span data-stu-id="a89bc-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="a89bc-110">يتم إرسال لمسؤولي مجموعة الموقع ولكن ليس للمستخدمين الآخرين بالبريد الإلكتروني من مهام سير العمل ومشاهدة الخطأ **HTTP محظور ل <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="a89bc-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="a89bc-111">راجع [رفض الوصول عند إرسال رسالة بريد إلكتروني لمجموعة SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="a89bc-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="a89bc-112">تحقق أيضا من ميزة مجموعة موقع **الوصول المحدود إلى وضع تأمين إذن المستخدم** غير نشط.</span><span class="sxs-lookup"><span data-stu-id="a89bc-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="a89bc-113">المواضيع ذات الصلة</span><span class="sxs-lookup"><span data-stu-id="a89bc-113">Related topics</span></span>
<span data-ttu-id="a89bc-114">هل ترغب في محاولة تدفق Microsoft SharePoint على الإنترنت؟</span><span class="sxs-lookup"><span data-stu-id="a89bc-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="a89bc-115">إنشاء تدفق</span><span class="sxs-lookup"><span data-stu-id="a89bc-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="a89bc-116">SharePoint والتدفق</span><span class="sxs-lookup"><span data-stu-id="a89bc-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


