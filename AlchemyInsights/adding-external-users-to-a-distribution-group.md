---
title: إضافة مستخدمين خارجيين إلى مجموعة توزيع
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 7dbc69bced9ca800d3f95081b77dda5e49662579
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/27/2020
ms.locfileid: "43910919"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="f92c2-102">إضافة مستخدمين خارجيين إلى مجموعة توزيع</span><span class="sxs-lookup"><span data-stu-id="f92c2-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="f92c2-103">إضافة جهة اتصال خارجية إلى مجموعة توزيع (DG) هي عملية من خطوتين:</span><span class="sxs-lookup"><span data-stu-id="f92c2-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="f92c2-104">إنشاء جهة اتصال بريد للمستخدم الخارجي:</span><span class="sxs-lookup"><span data-stu-id="f92c2-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="f92c2-105">في مركز المشرف، انتقل إلى صفحة[جهات اتصال](https://admin.microsoft.com/adminportal/home#/Contact) **المستخدمين.** > </span><span class="sxs-lookup"><span data-stu-id="f92c2-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="f92c2-106">حدد **إضافة جهة اتصال**.</span><span class="sxs-lookup"><span data-stu-id="f92c2-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="f92c2-107">اكتب المعلومات الخاصة بجهة الاتصال الخاصة بك وحدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="f92c2-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="f92c2-108">إضافة جهة اتصال البريد إلى DG الخاص بك:</span><span class="sxs-lookup"><span data-stu-id="f92c2-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="f92c2-109">في مركز المسؤول، انتقل إلى صفحة[مجموعات](https://admin.microsoft.com/adminportal/home#/groups) **المجموعات.** > </span><span class="sxs-lookup"><span data-stu-id="f92c2-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="f92c2-110">ابحث عن DG الذي تريد إضافة المستخدم الخارجي إليه، وحدده لفتح مربع حوار تحرير.</span><span class="sxs-lookup"><span data-stu-id="f92c2-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="f92c2-111">في علامة التبويب **الأعضاء،** حدد **عرض الكل وإدارة الأعضاء**.</span><span class="sxs-lookup"><span data-stu-id="f92c2-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="f92c2-112">حدد **إضافة أعضاء**.</span><span class="sxs-lookup"><span data-stu-id="f92c2-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="f92c2-113">حدد جهة اتصال البريد التي أنشأتها في الخطوة السابقة، ثم حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="f92c2-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="f92c2-114">إذا لم يتمكن المستخدمون الخارجيون بعد اتباع هذه الخطوات من إرسال رسائل البريد الإلكتروني إلى DG أو لم يتلقوا رسائل بريد إلكتروني منه، فقد يكون ذلك أن يتم وضع علامة على DG للسماح فقط برسائل البريد الإلكتروني من المستخدمين الداخليين.</span><span class="sxs-lookup"><span data-stu-id="f92c2-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="f92c2-115">يمكنك التحقق من هذا التكوين وإصلاحه باتباع الاتجاهات [هنا](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="f92c2-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="f92c2-116">**ملاحظة:** لا تنطبق هذه الإرشادات إذا كان نوع مجموعتك هو "مجموعة Microsoft 365" بدلاً من "مجموعة التوزيع".</span><span class="sxs-lookup"><span data-stu-id="f92c2-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="f92c2-117">إذا كان هذا هو الحال، يمكنك إضافة المستخدم الخارجي مباشرة إلى المجموعة من Outlook.</span><span class="sxs-lookup"><span data-stu-id="f92c2-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="f92c2-118">يمكن العثور على معلومات تفصيلية عن ضيوف مجموعات Microsoft 365 بالإضافة إلى إرشادات لإضافة ضيوف خارجيين في [هذه المقالة](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="f92c2-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  