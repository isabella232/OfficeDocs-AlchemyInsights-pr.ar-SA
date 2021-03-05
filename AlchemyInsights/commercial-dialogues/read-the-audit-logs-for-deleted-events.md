---
title: قراءة سجلات التدقيق للأحداث المحذوفة
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
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/05/2021
ms.locfileid: "50480885"
---
# <a name="read-the-audit-logs-for-deleted-events"></a><span data-ttu-id="ae2f0-102">قراءة سجلات التدقيق للأحداث المحذوفة</span><span class="sxs-lookup"><span data-stu-id="ae2f0-102">Read the audit logs for deleted events</span></span>

<span data-ttu-id="ae2f0-103">إليك كيفية القيام بذلك:</span><span class="sxs-lookup"><span data-stu-id="ae2f0-103">Here's how to do this:</span></span>

1. <span data-ttu-id="ae2f0-104">انتقل إلى مركز التوافق في [Office 365 &.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="ae2f0-104">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="ae2f0-105">حدد **البحث**  >  [**في سجل تدقيق البحث.**](https://go.microsoft.com/fwlink/?linkid=2103759)</span><span class="sxs-lookup"><span data-stu-id="ae2f0-105">Select **Search** > [**Audit log search**](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>
    > [!NOTE]
    > <span data-ttu-id="ae2f0-106">إذا رأيت إشعارا بأنه يجب تشغيل الميزة، فمضي قدما وقلبها الآن.</span><span class="sxs-lookup"><span data-stu-id="ae2f0-106">If you see a notice that you need to turn on the feature, go ahead and turn it on now.</span></span> <span data-ttu-id="ae2f0-107">إذا لم يتم تشغيل الميزة، فلن تتمكن نتائج البحث من سحب البيانات من التواريخ السابقة.</span><span class="sxs-lookup"><span data-stu-id="ae2f0-107">If the feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="ae2f0-108">حدد **"الأنشطة"،** ثم ابحث عن أنشطة **علبة بريد Exchange.**</span><span class="sxs-lookup"><span data-stu-id="ae2f0-108">Select **Activities**, and then find **Exchange mailbox activities**.</span></span> <span data-ttu-id="ae2f0-109">حدد الرسائل **المحذوفة من** مجلد "العناصر المحذوفة" والرسائل التي تم نقلها إلى خيارات مجلد **"العناصر** المحذوفة".</span><span class="sxs-lookup"><span data-stu-id="ae2f0-109">Select the **Deleted messages from Deleted Items** folder and **Moved messages to Deleted Items** folder options.</span></span> <span data-ttu-id="ae2f0-110">عندما تنتهي، انقر خارج الجزء لتصغير **جزء** "الأنشطة".</span><span class="sxs-lookup"><span data-stu-id="ae2f0-110">When you're done, click outside of the pane to minimize the **Activities** pane.</span></span>
1. <span data-ttu-id="ae2f0-111">حدد نطاق التاريخ، ثم  في المربع "المستخدمون"، حدد اسم المستخدم للمستخدم الذي تريد التحقق منه.</span><span class="sxs-lookup"><span data-stu-id="ae2f0-111">Specify the date range, and then in the **Users** box, select the username for the user you want to investigate.</span></span> <span data-ttu-id="ae2f0-112">يمكنك تحديد أكثر من مستخدم واحد في كل مرة.</span><span class="sxs-lookup"><span data-stu-id="ae2f0-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="ae2f0-113">حدد **"بحث".**</span><span class="sxs-lookup"><span data-stu-id="ae2f0-113">Select **Search**.</span></span> <span data-ttu-id="ae2f0-114">تظهر الأنشطة ضمن **"النتائج".**</span><span class="sxs-lookup"><span data-stu-id="ae2f0-114">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="ae2f0-115">لعرض التفاصيل، حدد نشاطا، ثم حدد **"مزيد من المعلومات".**</span><span class="sxs-lookup"><span data-stu-id="ae2f0-115">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="ae2f0-116">يتم عرض معلومات إضافية حول العنصر المحذوف، مثل سطر الموضوع وموقع العنصر عند حذفه، في الحقل **AffectedItems.**</span><span class="sxs-lookup"><span data-stu-id="ae2f0-116">Additional information about the deleted item, such as the subject line and the location of the item when it was deleted, is displayed in the **AffectedItems** field.</span></span>
    > [!NOTE]
    > <span data-ttu-id="ae2f0-117">لا يمكنك استعادة العناصر المحذوفة باستخدام ميزة سجل التدقيق.</span><span class="sxs-lookup"><span data-stu-id="ae2f0-117">You can't restore deleted items using the audit log feature.</span></span> <span data-ttu-id="ae2f0-118">لاستعادة العناصر المحذوفة، راجع استرداد العناصر المحذوفة أو البريد الإلكتروني المحذوف [في Outlook Web App.](https://go.microsoft.com/fwlink/?linkid=2103759)</span><span class="sxs-lookup"><span data-stu-id="ae2f0-118">To restore deleted items, see [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>

<span data-ttu-id="ae2f0-119">لمعرفة المزيد، راجع البحث في سجل تدقيق Office 365 استكشاف الأخطاء [وإصلاحها في السيناريوهات الشائعة.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="ae2f0-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
