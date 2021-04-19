---
title: إنشاء نهج مشاركة للسماح للمستخدمين بمشاركة تقويمهم مع أشخاص من خارج مؤسستك
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 016b915a9e8f7e32d5d393bc47347991866647c7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816259"
---
# <a name="create-a-sharing-policy-to-allow-your-users-to-share-their-calendar-with-people-outside-your-organization"></a><span data-ttu-id="49f2c-102">إنشاء نهج مشاركة للسماح للمستخدمين بمشاركة تقويمهم مع أشخاص من خارج مؤسستك</span><span class="sxs-lookup"><span data-stu-id="49f2c-102">Create a Sharing Policy to allow your users to share their calendar with people outside your organization</span></span>

1. <span data-ttu-id="49f2c-103">من لوحة معلومات مركز إدارة Microsoft 365، انتقل إلى **Exchange**  >  **المسؤول**.</span><span class="sxs-lookup"><span data-stu-id="49f2c-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="49f2c-104">انتقل إلى **مشاركة**  >  **المؤسسة**.</span><span class="sxs-lookup"><span data-stu-id="49f2c-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="49f2c-105">في طريقة عرض القائمة، ضمن **مشاركة فردية،** انقر فوق **جديد** .</span><span class="sxs-lookup"><span data-stu-id="49f2c-105">In the list view, under **Individual Sharing**, click **New** .</span></span>
4. <span data-ttu-id="49f2c-106">في **نهج المشاركة الجديد**، اكتب اسما ودودا لنهية المشاركة في المربع **اسم** النهج.</span><span class="sxs-lookup"><span data-stu-id="49f2c-106">In **new sharing policy**, type a friendly name for the sharing policy in the **Policy name** box.</span></span>
5. <span data-ttu-id="49f2c-107">انقر **فوق**  إضافة لتعريف قواعد المشاركة للنقرة.</span><span class="sxs-lookup"><span data-stu-id="49f2c-107">Click **Add**  to define the sharing rules for the policy.</span></span>
6. <span data-ttu-id="49f2c-108">في **قاعدة المشاركة**، حدد أحد الخيارات التالية لتحديد المجالات التي تريد المشاركة معها:</span><span class="sxs-lookup"><span data-stu-id="49f2c-108">In **sharing rule**, select one of the following options to specify the domains you want to share with:</span></span>
    - <span data-ttu-id="49f2c-109">**المشاركة مع كل المجالات**</span><span class="sxs-lookup"><span data-stu-id="49f2c-109">**Sharing with all domains**</span></span>
    - <span data-ttu-id="49f2c-110">**المشاركة مع مجال معين**</span><span class="sxs-lookup"><span data-stu-id="49f2c-110">**Sharing with a specific domain**</span></span>
8. <span data-ttu-id="49f2c-111">إذا حددت **مشاركة مع مجال معين،** فا اكتب اسم المجال الذي تريد المشاركة معه.</span><span class="sxs-lookup"><span data-stu-id="49f2c-111">If you select **Sharing with a specific domain**, type the name of the domain you want to share with.</span></span> <span data-ttu-id="49f2c-112">إذا كنت بحاجة إلى إدخال أكثر من مجال واحد لن نهج المشاركة هذا، فاحفظ إعدادات المجال الأول، ثم قم بتحرير قواعد المشاركة لإضافة المزيد من المجالات.</span><span class="sxs-lookup"><span data-stu-id="49f2c-112">If you need to enter more than one domain for this sharing policy, save the settings for the first domain, then edit the sharing rules to add more domains.</span></span>
9. <span data-ttu-id="49f2c-113">لتحديد المعلومات التي يمكن مشاركتها،  حدد خانة الاختيار مشاركة مجلد التقويم، ثم حدد أحد الخيارات التالية:</span><span class="sxs-lookup"><span data-stu-id="49f2c-113">To specify the information that can be shared, select the **Share your calendar folder** check box, and then select one of the following options:</span></span>
    - <span data-ttu-id="49f2c-114">**معلومات الازدحام/الانشغال في التقويم مع الوقت فقط**</span><span class="sxs-lookup"><span data-stu-id="49f2c-114">**Calendar free/busy information with time only**</span></span>
    - <span data-ttu-id="49f2c-115">**معلومات الازدحام/الانشغال في التقويم مع الوقت والموضوع والموقع**</span><span class="sxs-lookup"><span data-stu-id="49f2c-115">**Calendar free/busy information with time, subject, and location**</span></span>
    - <span data-ttu-id="49f2c-116">**كل معلومات موعد التقويم، بما في ذلك الوقت والموضوع والموقع والملقب**</span><span class="sxs-lookup"><span data-stu-id="49f2c-116">**All calendar appointment information, including time, subject, location and title**</span></span>
11. <span data-ttu-id="49f2c-117">انقر **فوق** حفظ لتعيين قواعد نهج المشاركة.</span><span class="sxs-lookup"><span data-stu-id="49f2c-117">Click **save** to set the rules for the sharing policy.</span></span>
12. <span data-ttu-id="49f2c-118">إذا كنت تريد تعيين نهج المشاركة هذا ك نهج المشاركة الافتراضي الجديد لجميع المستخدمين في مؤسستك، فحدد خانة الاختيار جعل هذا النهج نهج المشاركة **الافتراضي** الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="49f2c-118">If you want to set this sharing policy as the new default sharing policy for all users in your organization, select the **Make this policy my default sharing policy** check box.</span></span>
13. <span data-ttu-id="49f2c-119">انقر **فوق** حفظ لإنشاء نهج المشاركة.</span><span class="sxs-lookup"><span data-stu-id="49f2c-119">Click **save** to create the sharing policy.</span></span>  

<span data-ttu-id="49f2c-120">**للتوصل إلى فهم كامل لهذا الموضوع، رجاءً اقرأ:**</span><span class="sxs-lookup"><span data-stu-id="49f2c-120">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="49f2c-121">إنشاء نهج مشاركة في Exchange Online</span><span class="sxs-lookup"><span data-stu-id="49f2c-121">Create a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/create-a-sharing-policy)
- [<span data-ttu-id="49f2c-122">تطبيق نهج مشاركة على علب البريد في Exchange Online</span><span class="sxs-lookup"><span data-stu-id="49f2c-122">Apply a sharing policy to mailboxes in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy)
- [<span data-ttu-id="49f2c-123">تعديل نهج مشاركة أو تعطيله أو إزالته في Exchange Online</span><span class="sxs-lookup"><span data-stu-id="49f2c-123">Modify, disable, or remove a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)