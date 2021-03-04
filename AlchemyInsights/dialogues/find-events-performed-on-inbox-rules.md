---
title: البحث عن الأحداث التي تم تنفيذها على قواعد علبة الوارد
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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429249"
---
# <a name="find-events-performed-on-inbox-rules"></a><span data-ttu-id="baa4e-102">البحث عن الأحداث التي تم تنفيذها على قواعد علبة الوارد</span><span class="sxs-lookup"><span data-stu-id="baa4e-102">Find events performed on inbox rules</span></span>

<span data-ttu-id="baa4e-103">عند إنشاء قواعد علبة الوارد أو تغييرها أو حذفها، يتم تسجيل الأحداث في سجل التدقيق.</span><span class="sxs-lookup"><span data-stu-id="baa4e-103">When inbox rules are created, changed, or deleted, the events are recorded in the audit log.</span></span> <span data-ttu-id="baa4e-104">فيما يلي كيفية مراجعتها:</span><span class="sxs-lookup"><span data-stu-id="baa4e-104">Here's how to review them:</span></span>

1. <span data-ttu-id="baa4e-105">انتقل إلى مركز التوافق في [Office 365 &.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="baa4e-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="baa4e-106">حدد البحث > البحث في سجل التدقيق.</span><span class="sxs-lookup"><span data-stu-id="baa4e-106">Select Search > Audit log search.</span></span>

    > [!NOTE]
    > <span data-ttu-id="baa4e-107">إذا رأيت إشعارا بأنه يجب تشغيل التدقيق، فمضي قدما وقلبه الآن.</span><span class="sxs-lookup"><span data-stu-id="baa4e-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="baa4e-108">إذا لم يتم تشغيل هذه الميزة، فلن تتمكن نتائج البحث من سحب البيانات من التواريخ السابقة.</span><span class="sxs-lookup"><span data-stu-id="baa4e-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="baa4e-109">حدد حقل "الأنشطة" واعثر على أنشطة علبة بريد Exchange، ثم حدد New-InboxRule قاعدة "إنشاء علبة الوارد" من Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="baa4e-109">Select the Activities field and find Exchange mailbox activities, and then select New-InboxRule Create inbox rule from Outlook Web App.</span></span> <span data-ttu-id="baa4e-110">عندما تنتهي، انقر خارج الجزء لتصغير جزء "الأنشطة".</span><span class="sxs-lookup"><span data-stu-id="baa4e-110">When you're done, click outside of the pane to minimize the Activities pane.</span></span>
1. <span data-ttu-id="baa4e-111">حدد نطاق التاريخ، ثم في حقل "المستخدمون"، حدد اسم المستخدم للمستخدم الذي تريد التحقق منه.</span><span class="sxs-lookup"><span data-stu-id="baa4e-111">Specify the date range, and then in the Users field, select the username for the user you want to investigate.</span></span> <span data-ttu-id="baa4e-112">يمكنك تحديد أكثر من مستخدم واحد في كل مرة.</span><span class="sxs-lookup"><span data-stu-id="baa4e-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="baa4e-113">حدد "بحث".</span><span class="sxs-lookup"><span data-stu-id="baa4e-113">Select Search.</span></span> <span data-ttu-id="baa4e-114">تظهر الأنشطة ضمن "النتائج".</span><span class="sxs-lookup"><span data-stu-id="baa4e-114">The activities appear under Results.</span></span>
1. <span data-ttu-id="baa4e-115">لعرض التفاصيل، حدد نشاطا، ثم حدد "مزيد من المعلومات".</span><span class="sxs-lookup"><span data-stu-id="baa4e-115">To view details, select an activity, and then select More Information.</span></span> <span data-ttu-id="baa4e-116">ضمن القسم "معلمات"، يمكنك رؤية اسم القاعدة، مجموعة الشروط، والإجراءات التي ستتخذها القاعدة.</span><span class="sxs-lookup"><span data-stu-id="baa4e-116">Under the Parameters section you can see the name of the rule, conditions set, and the actions that the rule will take.</span></span>

<span data-ttu-id="baa4e-117">لمعرفة المزيد، راجع "البحث في سجل تدقيق Office 365" للتعرف على السيناريوهات الشائعة وإصلاحها.</span><span class="sxs-lookup"><span data-stu-id="baa4e-117">To learn more, see Search the Office 365 audit log to troubleshoot common scenarios.</span></span>