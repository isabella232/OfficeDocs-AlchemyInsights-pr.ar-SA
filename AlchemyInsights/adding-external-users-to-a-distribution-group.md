---
title: إضافة المستخدمين الخارجيين إلى مجموعة التوزيع؟
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 8/22/2017
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: a5def36fbb662037851158722db60494f00ce850
ms.sourcegitcommit: a9be2e396022382e92cf40c0d0d82f2f59c2e259
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/12/2019
ms.locfileid: "34895192"
---
# <a name="adding-external-users-to-a-distribution-group"></a><span data-ttu-id="25558-102">إضافة المستخدمين الخارجيين إلى مجموعة التوزيع؟</span><span class="sxs-lookup"><span data-stu-id="25558-102">Adding external users to a Distribution Group?</span></span>

<span data-ttu-id="25558-103">إضافة جهة اتصال خارجي لمجموعة التوزيع (DG) عملية من خطوتين:</span><span class="sxs-lookup"><span data-stu-id="25558-103">Adding an external contact to a Distribution Group (DG) is a 2-step process:</span></span>
  
1. <span data-ttu-id="25558-104">إنشاء جهة "اتصال بريد" للمستخدمين الخارجيين:</span><span class="sxs-lookup"><span data-stu-id="25558-104">Create a Mail Contact for the external user:</span></span>
    
1. <span data-ttu-id="25558-105">انقر [هنا](https://admin.microsoft.com/adminportal/home#/Contact) للانتقال إلى الصفحة تحرير جهة الاتصال في مدخل مسؤول.</span><span class="sxs-lookup"><span data-stu-id="25558-105">Click [here](https://admin.microsoft.com/adminportal/home#/Contact) to navigate to the Contact edit page in the Admin portal.</span></span> 
    
2. <span data-ttu-id="25558-106">انقر فوق **إضافة جهة اتصال**.</span><span class="sxs-lookup"><span data-stu-id="25558-106">Click on **Add a Contact**.</span></span>
    
3. <span data-ttu-id="25558-107">اكتب المعلومات الخاصة بجهة الاتصال، ثم انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="25558-107">Type the information for your contact and click **Save**.</span></span>
    
2. <span data-ttu-id="25558-108">إضافة جهة اتصال بريد إلى المديرية العامة الخاصة بك:</span><span class="sxs-lookup"><span data-stu-id="25558-108">Add the Mail Contact to your DG:</span></span>
    
1. <span data-ttu-id="25558-109">انقر [هنا](https://admin.microsoft.com/adminportal/home#/groups) للانتقال إلى صفحة المجموعات.</span><span class="sxs-lookup"><span data-stu-id="25558-109">Click [here](https://admin.microsoft.com/adminportal/home#/groups) to navigate to the Groups page.</span></span> 
    
2. <span data-ttu-id="25558-110">البحث عن المدير العام الذي تريد إضافة مستخدم خارجي إلى، انقر فوقه لفتح مربع الحوار تحرير.</span><span class="sxs-lookup"><span data-stu-id="25558-110">Find the DG you want to add the external user to, and click on it to open the edit dialog.</span></span>
    
3. <span data-ttu-id="25558-111">انقر فوق الزر **تحرير** في قائمة **الأعضاء** .</span><span class="sxs-lookup"><span data-stu-id="25558-111">Click on the **Edit** button in the **Members** list.</span></span> 
    
4. <span data-ttu-id="25558-112">انقر فوق **إضافة أعضاء**.</span><span class="sxs-lookup"><span data-stu-id="25558-112">Click on **Add Members**.</span></span>
    
5. <span data-ttu-id="25558-113">حدد "جهة اتصال بريد" قمت بإنشائه في الخطوة السابقة، ثم انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="25558-113">Select the Mail Contact you created on the previous step and click **Save**.</span></span>
    
<span data-ttu-id="25558-114">إذا حتى بعد اتباع هذه الخطوات لا يمكن إرسال رسائل البريد الإلكتروني إلى المدير العام الخاص بك المستخدمين الخارجيين أو عدم استلام رسائل البريد الإلكتروني منه، يمكن أن يتم تمييز المدير العام للسماح بالبريد الإلكتروني فقط من المستخدمين الداخليين.</span><span class="sxs-lookup"><span data-stu-id="25558-114">If even after following these steps your external users can't send emails to the DG or don't receive emails from it, it can be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="25558-115">يمكنك التحقق من هذا التكوين وإصلاحها اتباع الإرشادات [هنا](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx)</span><span class="sxs-lookup"><span data-stu-id="25558-115">You can check this configuration and fix it following the directions [here](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx)</span></span>
  
 <span data-ttu-id="25558-116">**ملاحظة:** لا تنطبق هذه التعليمات إذا كان نوع المجموعة الخاصة بك "جماعة Office 365" بدلاً من "مجموعة التوزيع".</span><span class="sxs-lookup"><span data-stu-id="25558-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="25558-117">إذا كان الأمر كذلك، يمكنك إضافة المستخدم الخارجي مباشرة إلى المجموعة من Outlook أو Outlook على الويب.</span><span class="sxs-lookup"><span data-stu-id="25558-117">If that is the case, you can add the external user directly to the group from Outlook or Outlook on the Web.</span></span> <span data-ttu-id="25558-118">يمكن العثور على شرح مفصل على الضيوف مجموعات O365 وكذلك الإرشادات لإضافة ضيوف الخارجية في [هذه المقالة](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="25558-118">Detailed explanation on O365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  