---
title: إضافة المستخدمين الخارجيين إلى مجموعة التوزيع
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 8/22/2017
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: ce0c589e1661fb4607452fe2e8f897758b2718e8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36494514"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="714c1-102">إضافة المستخدمين الخارجيين إلى مجموعة التوزيع؟</span><span class="sxs-lookup"><span data-stu-id="714c1-102">Add external users to a Distribution Group?</span></span>

<span data-ttu-id="714c1-103">إضافة جهة اتصال خارجي لمجموعة التوزيع (DG) عملية من خطوتين:</span><span class="sxs-lookup"><span data-stu-id="714c1-103">Adding an external contact to a Distribution Group (DG) is a 2-step process:</span></span>
  
1. <span data-ttu-id="714c1-104">إنشاء جهة "اتصال بريد" للمستخدمين الخارجيين:</span><span class="sxs-lookup"><span data-stu-id="714c1-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="714c1-105">في مركز الإدارة، انتقل إلى **المستخدمين** > الصفحة[جهات الاتصال](https://admin.microsoft.com/adminportal/home#/Contact) .</span><span class="sxs-lookup"><span data-stu-id="714c1-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="714c1-106">حدد **إضافة جهة اتصال**.</span><span class="sxs-lookup"><span data-stu-id="714c1-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="714c1-107">اكتب المعلومات الخاصة بجهة الاتصال، ثم اختر **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="714c1-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="714c1-108">إضافة جهة اتصال بريد إلى المديرية العامة الخاصة بك:</span><span class="sxs-lookup"><span data-stu-id="714c1-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="714c1-109">في مركز الإدارة، انتقل إلى **مجموعات** > صفحة[مجموعات](https://admin.microsoft.com/adminportal/home#/groups) .</span><span class="sxs-lookup"><span data-stu-id="714c1-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="714c1-110">البحث الذي تريد إضافة مستخدم خارجي إلى المدير العام، وتحديدها لفتح مربع الحوار تحرير.</span><span class="sxs-lookup"><span data-stu-id="714c1-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="714c1-111">علامة التبويب **الأعضاء** ، حدد **عرض كافة وإدارة الأعضاء**.</span><span class="sxs-lookup"><span data-stu-id="714c1-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="714c1-112">حدد **إضافة أعضاء**.</span><span class="sxs-lookup"><span data-stu-id="714c1-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="714c1-113">حدد "جهة اتصال بريد" قمت بإنشائه في الخطوة السابقة، وحدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="714c1-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="714c1-114">بعد اتباع هذه الخطوات المستخدمين الخارجيين لا يمكن إرسال رسائل البريد الإلكتروني إلى المدير العام أو عدم استلام رسائل البريد الإلكتروني منه، قد يكون تم وضع علامة المدير العام للسماح برسائل البريد الإلكتروني فقط من المستخدمين الداخليين.</span><span class="sxs-lookup"><span data-stu-id="714c1-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="714c1-115">يمكنك التحقق من هذا التكوين وإصلاحها اتباع الإرشادات [هنا](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).</span><span class="sxs-lookup"><span data-stu-id="714c1-115">You can check this configuration and fix it following the directions [here](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).</span></span>
  
 <span data-ttu-id="714c1-116">**ملاحظة:** لا تنطبق هذه التعليمات إذا كان نوع المجموعة الخاصة بك "جماعة Office 365" بدلاً من "مجموعة التوزيع".</span><span class="sxs-lookup"><span data-stu-id="714c1-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="714c1-117">إذا كان الأمر كذلك، يمكنك إضافة المستخدم الخارجي مباشرة إلى المجموعة من Outlook.</span><span class="sxs-lookup"><span data-stu-id="714c1-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="714c1-118">يمكن العثور على معلومات مفصلة عن الضيوف مجموعات Office 365 وكذلك الإرشادات لإضافة ضيوف الخارجية في [هذه المقالة](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="714c1-118">Detailed information on Office 365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  