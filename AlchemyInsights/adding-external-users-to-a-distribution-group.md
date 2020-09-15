---
title: أضافه مستخدمين خارجيين إلى مجموعه توزيع
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663500"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="8299c-102">أضافه مستخدمين خارجيين إلى مجموعه توزيع</span><span class="sxs-lookup"><span data-stu-id="8299c-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="8299c-103">تعد أضافه جهة اتصال خارجيه إلى مجموعه توزيع (توزيع) عمليه تتكون من خطوتين:</span><span class="sxs-lookup"><span data-stu-id="8299c-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="8299c-104">إنشاء جهة اتصال بريد للمستخدم الخارجي:</span><span class="sxs-lookup"><span data-stu-id="8299c-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="8299c-105">في مركز الاداره ، انتقل إلى صفحه **Users**  >  [جات اتصال](https://admin.microsoft.com/adminportal/home#/Contact) المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="8299c-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="8299c-106">حدد **أضافه جهة اتصال**.</span><span class="sxs-lookup"><span data-stu-id="8299c-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="8299c-107">اكتب المعلومات الخاصة بجهة الاتصال وحدد **أضافه**.</span><span class="sxs-lookup"><span data-stu-id="8299c-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="8299c-108">أضف جهة الاتصال الخاصة بالبريد إلى توزيعك:</span><span class="sxs-lookup"><span data-stu-id="8299c-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="8299c-109">في مركز الاداره ، انتقل إلى صفحه مجموعات **المجموعات**  >  [Groups](https://admin.microsoft.com/adminportal/home#/groups) .</span><span class="sxs-lookup"><span data-stu-id="8299c-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="8299c-110">ابحث عن توزيع الذي تريد أضافه المستخدم الخارجي اليه ، وحدده لفتح مربع الحوار تحرير.</span><span class="sxs-lookup"><span data-stu-id="8299c-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="8299c-111">علي علامة التبويب **الأعضاء** ، حدد **عرض كل الأعضاء وأدارهم**.</span><span class="sxs-lookup"><span data-stu-id="8299c-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="8299c-112">حدد **أضافه أعضاء**.</span><span class="sxs-lookup"><span data-stu-id="8299c-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="8299c-113">حدد جهة الاتصال التي انشاتها في الخطوة السابقة ، ثم حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="8299c-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="8299c-114">إذا لم يتمكن المستخدمون الخارجيون من تنفيذ الخطوات التالية من إرسال رسائل البريد الكتروني إلى توزيع أو عدم تلقي رسائل البريد الكتروني منه ، فقد يكون من الممكن وضع علامة علي التوزيع للسماح برسائل البريد الكتروني من المستخدمين الداخليين فقط.</span><span class="sxs-lookup"><span data-stu-id="8299c-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="8299c-115">يمكنك التحقق من هذا التكوين وإصلاحه باتباع الإرشادات الواردة [هنا](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="8299c-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="8299c-116">**ملاحظه:** لا تنطبق هذه الإرشادات إذا كان نوع المجموعة "Microsoft 365 group" بدلا من "مجموعه التوزيع".</span><span class="sxs-lookup"><span data-stu-id="8299c-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="8299c-117">إذا كانت هذه هي الحالة ، يمكنك أضافه المستخدم الخارجي مباشره إلى المجموعة من Outlook.</span><span class="sxs-lookup"><span data-stu-id="8299c-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="8299c-118">يمكن العثور علي معلومات مفصله حول ضيوف مجموعات Microsoft 365 بالاضافه إلى الإرشادات المتعلقة باضافه ضيوف خارجيين في [هذه المقالة](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="8299c-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  