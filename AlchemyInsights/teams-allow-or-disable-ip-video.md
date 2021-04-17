---
title: يسمح Teams بفيديو IP أو يعطله
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
- "9002537"
- "5617"
ms.openlocfilehash: 059d7a1ad619e25f14bc6f561693b6fe24355132
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826330"
---
# <a name="teams-allow-or-disable-ip-video"></a><span data-ttu-id="392b3-102">يسمح Teams بفيديو IP أو يعطله</span><span class="sxs-lookup"><span data-stu-id="392b3-102">Teams allow or disable IP video</span></span>

<span data-ttu-id="392b3-103">**تغيير نهج اجتماع أو إنشائه**</span><span class="sxs-lookup"><span data-stu-id="392b3-103">**Change or create a meeting policy**</span></span>

<span data-ttu-id="392b3-104">لتغيير نهج اجتماع أو إنشائه، انتقل إلى مركز إدارة Microsoft Teams > **الاجتماعات > نهج الاجتماعات.**</span><span class="sxs-lookup"><span data-stu-id="392b3-104">To change or create a meeting policy, go to the **Microsoft Teams admin center > Meetings > Meeting policies**.</span></span> <span data-ttu-id="392b3-105">حدد نهجاً من القائمة أو انقر فوق **إضافة**.</span><span class="sxs-lookup"><span data-stu-id="392b3-105">Select a policy from the list or click **Add**.</span></span> <span data-ttu-id="392b3-106">إذا كنت تقوم بإنشاء نهج جديد، فأضف اسماً ووصفاً.</span><span class="sxs-lookup"><span data-stu-id="392b3-106">If you're creating a new policy, add a name and description.</span></span> <span data-ttu-id="392b3-107">لا يمكن أن يحتوي الاسم على أحرف خاصة أو أن يكون أطول من 64 حرفاً.</span><span class="sxs-lookup"><span data-stu-id="392b3-107">The name can't contain special characters or be longer than 64 characters.</span></span> <span data-ttu-id="392b3-108">اختر الإعدادات الخاصة بك، ثم انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="392b3-108">Choose your settings, and then click **Save**.</span></span>

<span data-ttu-id="392b3-109">على سبيل المثال، لنقول أن لديك العديد من المستخدمين وتريد الحد من مقدار النطاق الترددي الذي يتطلبه اجتماعهم.</span><span class="sxs-lookup"><span data-stu-id="392b3-109">For example, say you have many users and you want to limit the amount of bandwidth that their meeting would require.</span></span> <span data-ttu-id="392b3-110">ستقوم بإنشاء نهج مخصص جديد باسم "النطاق الترددي المحدود" وتعطيل الإعدادات التالية:</span><span class="sxs-lookup"><span data-stu-id="392b3-110">You would create a new custom policy named "Limited bandwidth" and disable the following settings:</span></span>

<span data-ttu-id="392b3-111">ضمن **الصوت والفيديو**:</span><span class="sxs-lookup"><span data-stu-id="392b3-111">Under **Audio & video**:</span></span>

- <span data-ttu-id="392b3-112">قم بإيقاف تشغيل السماح بالتسجيل في السحابة.</span><span class="sxs-lookup"><span data-stu-id="392b3-112">Turn off Allow cloud recording.</span></span>
- <span data-ttu-id="392b3-113">قم بإيقاف تشغيل السماح بفيديو IP.</span><span class="sxs-lookup"><span data-stu-id="392b3-113">Turn off Allow IP video.</span></span>

<span data-ttu-id="392b3-114">بعد ذلك، قم بتعيين النهج إلى المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="392b3-114">Then assign the policy to the users.</span></span>

<span data-ttu-id="392b3-115">**تعيين نهج اجتماع للمستخدمين**</span><span class="sxs-lookup"><span data-stu-id="392b3-115">**Assign a meeting policy to users**</span></span>

1. <span data-ttu-id="392b3-116">في شريط التنقل الأيمن في مركز إدارة Microsoft Teams، انتقل إلى **المستخدمين**، ثم انقر فوق المستخدم.</span><span class="sxs-lookup"><span data-stu-id="392b3-116">In the left navigation of the Microsoft Teams admin center, go to **Users**, and then click the user.</span></span>
2. <span data-ttu-id="392b3-117">حدد المستخدم بالنقر إلى يمين اسم المستخدم ثم انقر فوق **تحرير الإعدادات**.</span><span class="sxs-lookup"><span data-stu-id="392b3-117">Select the user by clicking to the left of the user name, and then click **Edit settings**.</span></span>
3. <span data-ttu-id="392b3-118">ضمن **نهج الاجتماع،** حدد النهج الذي تريد تعيينه، ثم انقر فوق **تطبيق**.</span><span class="sxs-lookup"><span data-stu-id="392b3-118">Under **Meeting policy**, select the policy you want to assign and then click **Apply**.</span></span>

<span data-ttu-id="392b3-119">لمزيد من المعلومات، راجع [إدارة سياسات الاجتماعات في Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="392b3-119">For more information, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>
