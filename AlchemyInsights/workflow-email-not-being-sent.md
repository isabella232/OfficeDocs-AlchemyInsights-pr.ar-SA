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
ms.openlocfilehash: 783bf0a5721aa5db7088432c71e06cac6dc90513
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059591"
---
# <a name="workflow-email-is-not-being-sent"></a><span data-ttu-id="3f139-102">لم يتم إرسال البريد الإلكتروني سير العمل</span><span class="sxs-lookup"><span data-stu-id="3f139-102">Workflow email is not being sent</span></span>

1. <span data-ttu-id="3f139-103">لا يتم إرسال البريد الإلكتروني من مهام سير العمل لكافة المستخدمين أو مستخدمين معينين، أو ترى أنه لا يمكن إرسال خطأ **رسالة البريد الإلكتروني. تأكد من البريد الإلكتروني لمستلم صالح**.</span><span class="sxs-lookup"><span data-stu-id="3f139-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

<span data-ttu-id="3f139-104">معرفة ما إذا كان المستخدم موجوداً في مجموعة أذونات **كافة الأشخاص** (قائمة معلومات المستخدم) لمجموعة الموقع هذه.</span><span class="sxs-lookup"><span data-stu-id="3f139-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="3f139-105">نموذج عنوان URL مباشرة: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx؟ ميمبيرشيبجروبيد = 0</span><span class="sxs-lookup"><span data-stu-id="3f139-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

- <span data-ttu-id="3f139-106">إذا كان المستخدم غير موجود، تأكد من تسجيل المستخدم في الصفحة.</span><span class="sxs-lookup"><span data-stu-id="3f139-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
- <span data-ttu-id="3f139-107">إذا كان مستخدم خارجي، تأكد من أنه تم قبول الدعوة.</span><span class="sxs-lookup"><span data-stu-id="3f139-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
- <span data-ttu-id="3f139-108">إذا كان المستخدم موجود في مجموعة أذونات، تأكد من صحة عنوان البريد الإلكتروني.</span><span class="sxs-lookup"><span data-stu-id="3f139-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
- <span data-ttu-id="3f139-109">إذا لم يتم تعيين عنوان البريد الإلكتروني المستخدمين هنا، قم بإنشاء تنبيه كعينة لذلك المستخدم الذي يفرض المزامنة لحساب المستخدم هذا من التشكيلات الجانبية للمستخدم من SharePoint إلى مجموعة المواقع المشتركة هذه.</span><span class="sxs-lookup"><span data-stu-id="3f139-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="3f139-110">يتم إرسال لمسؤولي مجموعة الموقع ولكن ليس للمستخدمين الآخرين بالبريد الإلكتروني من مهام سير العمل ومشاهدة الخطأ \*\*HTTP محظور ل <spam> <spam> \*\* <spam> <spam>.</span><span class="sxs-lookup"><span data-stu-id="3f139-110">Email from Workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <spam><spam>https://URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**<spam><spam>.</span></span>
 

<span data-ttu-id="3f139-111">راجع [رفض الوصول عند تجميع رسائل البريد الإلكتروني المرسلة إلى](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="3f139-111">See [Access Denied when sent email to groups](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span></span>

<span data-ttu-id="3f139-112">تحقق أيضا من ميزة مجموعة موقع **الوصول المحدود إلى وضع تأمين إذن المستخدم** غير نشط.</span><span class="sxs-lookup"><span data-stu-id="3f139-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>

## <a name="related-topics"></a><span data-ttu-id="3f139-113">المواضيع ذات الصلة</span><span class="sxs-lookup"><span data-stu-id="3f139-113">Related topics</span></span>
- [<span data-ttu-id="3f139-114">إنشاء تدفق</span><span class="sxs-lookup"><span data-stu-id="3f139-114">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="3f139-115">SharePoint والتدفق</span><span class="sxs-lookup"><span data-stu-id="3f139-115">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


