---
title: إضافة مستخدمين خارجيين إلى مجموعة توزيع
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: e84a5b04d6fc805deaa47cb10c91081f37411e5b
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737860"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="e5bce-102">إضافة مستخدمين خارجيين إلى مجموعة توزيع</span><span class="sxs-lookup"><span data-stu-id="e5bce-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="e5bce-103">إضافة جهة اتصال خارجية إلى مجموعة توزيع (DG) عملية من خطوتين:</span><span class="sxs-lookup"><span data-stu-id="e5bce-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="e5bce-104">إنشاء جهة اتصال بريد للمستخدم الخارجي:</span><span class="sxs-lookup"><span data-stu-id="e5bce-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="e5bce-105">في مركز المسؤول، انتقل إلى صفحة["جهات اتصال](https://admin.microsoft.com/adminportal/home#/Contact) **المستخدمين".** > </span><span class="sxs-lookup"><span data-stu-id="e5bce-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="e5bce-106">حدد **إضافة جهة اتصال**.</span><span class="sxs-lookup"><span data-stu-id="e5bce-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="e5bce-107">اكتب المعلومات لجهة الاتصال الخاصة بك وحدد **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="e5bce-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="e5bce-108">إضافة جهة اتصال البريد إلى المديرية العامة:</span><span class="sxs-lookup"><span data-stu-id="e5bce-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="e5bce-109">في مركز المسؤول، انتقل إلى صفحة[مجموعات](https://admin.microsoft.com/adminportal/home#/groups) **المجموعات.** > </span><span class="sxs-lookup"><span data-stu-id="e5bce-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="e5bce-110">ابحث عن المدير ية التي تريد إضافة المستخدم الخارجي إليها، وحددها لفتح مربع حوار التحرير.</span><span class="sxs-lookup"><span data-stu-id="e5bce-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="e5bce-111">في علامة التبويب **الأعضاء،** حدد **عرض الكل وإدارة الأعضاء**.</span><span class="sxs-lookup"><span data-stu-id="e5bce-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="e5bce-112">حدد **إضافة أعضاء**.</span><span class="sxs-lookup"><span data-stu-id="e5bce-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="e5bce-113">حدد جهة اتصال البريد التي قمت بإنشائها في الخطوة السابقة، ثم حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="e5bce-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="e5bce-114">إذا لم يتمكن المستخدمون الخارجيون بعد اتباع هذه الخطوات من إرسال رسائل بريد إلكتروني إلى المديرية العامة أو عدم تلقي رسائل البريد الإلكتروني منها، فقد يكون من الممكن وضع علامة على المديرية العامة للسماح برسائل البريد الإلكتروني من المستخدمين الداخليين فقط.</span><span class="sxs-lookup"><span data-stu-id="e5bce-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="e5bce-115">يمكنك التحقق من هذا التكوين وإصلاحه باتباع الإرشادات [هنا](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="e5bce-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="e5bce-116">**ملاحظة:** لا يتم تطبيق هذه الإرشادات إذا كان نوع المجموعة الخاصة بك هو "مجموعة Office 365" بدلاً من "مجموعة التوزيع".</span><span class="sxs-lookup"><span data-stu-id="e5bce-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="e5bce-117">إذا كانت هذه هي الحالة، يمكنك إضافة المستخدم الخارجي مباشرة إلى المجموعة من Outlook.</span><span class="sxs-lookup"><span data-stu-id="e5bce-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="e5bce-118">يمكن العثور على معلومات مفصلة عن ضيوف مجموعات Office 365 وكذلك إرشادات لإضافة ضيوف خارجيين في [هذه المقالة](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="e5bce-118">Detailed information on Office 365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  