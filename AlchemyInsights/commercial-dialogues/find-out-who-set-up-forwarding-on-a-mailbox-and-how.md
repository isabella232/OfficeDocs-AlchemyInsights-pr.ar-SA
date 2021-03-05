---
title: تعرف على من قام بإعداد إعادة توجيه علبة بريد، وكيفية
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/05/2021
ms.locfileid: "50480889"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a><span data-ttu-id="65702-102">تعرف على من قام بإعداد إعادة توجيه على علبة بريد، وكيفية</span><span class="sxs-lookup"><span data-stu-id="65702-102">Find out who set up forwarding on a mailbox, and how</span></span>

<span data-ttu-id="65702-103">إذا تم تعيين إعادة توجيه خارجية على علبة بريد، فيتم تدقيق النشاط كجزء من Set-Mailbox cmdlet.</span><span class="sxs-lookup"><span data-stu-id="65702-103">If external forwarding was set on a mailbox, the activity is audited as part of the Set-Mailbox cmdlet.</span></span> <span data-ttu-id="65702-104">فيما يلي كيفية العثور على النشاط في سجل التدقيق:</span><span class="sxs-lookup"><span data-stu-id="65702-104">Here's how to find the activity in the audit log:</span></span>

1. <span data-ttu-id="65702-105">انتقل إلى مركز التوافق في [Office 365 &.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="65702-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="65702-106">حدد **البحث** >  **في سجل تدقيق البحث.**</span><span class="sxs-lookup"><span data-stu-id="65702-106">Select **Search**> **Audit log search**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="65702-107">إذا رأيت إشعارا بأنه يجب تشغيل التدقيق، فمضي قدما وقلبه الآن.</span><span class="sxs-lookup"><span data-stu-id="65702-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="65702-108">إذا لم يتم تشغيل هذه الميزة، فلن تتمكن نتائج البحث من سحب البيانات من التواريخ السابقة.</span><span class="sxs-lookup"><span data-stu-id="65702-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="65702-109">تأكد من تعيين الحقل **"أنشطة"** **إلى "إظهار النتائج" لكل الأنشطة** (الإعداد الافتراضي).</span><span class="sxs-lookup"><span data-stu-id="65702-109">Make sure the **Activities** field is set to **Show results for all activities** (the default).</span></span> <span data-ttu-id="65702-110">حدد نطاق التاريخ.</span><span class="sxs-lookup"><span data-stu-id="65702-110">Specify the date range.</span></span> <span data-ttu-id="65702-111">لست بحاجة إلى تحديد اسم مستخدم.</span><span class="sxs-lookup"><span data-stu-id="65702-111">You don't need to specify a username.</span></span>
1. <span data-ttu-id="65702-112">حدد **"بحث".**</span><span class="sxs-lookup"><span data-stu-id="65702-112">Select **Search**.</span></span> <span data-ttu-id="65702-113">تظهر الأنشطة ضمن **"النتائج".**</span><span class="sxs-lookup"><span data-stu-id="65702-113">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="65702-114">حدد **"تصفية النتائج"،** ثم أدخل **"مجموعة علبة البريد"** في **حقل عامل تصفية** "النشاط".</span><span class="sxs-lookup"><span data-stu-id="65702-114">Select **Filter Results**, and then enter **Set-mailbox** in the **Activity** filter field.</span></span> <span data-ttu-id="65702-115">يرجع هذا كل **أنشطة "مجموعة علبة** البريد".</span><span class="sxs-lookup"><span data-stu-id="65702-115">This returns all **Set-Mailbox** activities.</span></span>
1. <span data-ttu-id="65702-116">لعرض التفاصيل، حدد نشاطا، ثم حدد **"مزيد من المعلومات".**</span><span class="sxs-lookup"><span data-stu-id="65702-116">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="65702-117">ضمن **المعلمات،** يمكنك رؤية عنوان البريد الإلكتروني إعادة توجيه الذي تم تعيينه على علبة البريد.</span><span class="sxs-lookup"><span data-stu-id="65702-117">Under **Parameters** you can see the forwarding email address that was set on the mailbox.</span></span> <span data-ttu-id="65702-118">يمثل **UserID** المستخدم الذي قام بإعداد إعادة توجيه خارجية في علبة البريد.</span><span class="sxs-lookup"><span data-stu-id="65702-118">The **UserID** represents the user who set up external forwarding on the mailbox.</span></span>
<span data-ttu-id="65702-119">لمعرفة المزيد، راجع البحث في سجل تدقيق Office 365 استكشاف الأخطاء [وإصلاحها في السيناريوهات الشائعة.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="65702-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>