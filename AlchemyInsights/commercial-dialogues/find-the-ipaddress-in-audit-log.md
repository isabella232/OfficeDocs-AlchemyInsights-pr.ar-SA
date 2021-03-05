---
title: البحث عن عنوان IP في سجل التدقيق
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
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/05/2021
ms.locfileid: "50480928"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="47f92-102">البحث عن عنوان IP في سجل التدقيق</span><span class="sxs-lookup"><span data-stu-id="47f92-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="47f92-103">يظهر عنوان IP الذي يتطابق مع نشاط يقوم به مستخدم أو مسؤول في سجلات التدقيق.</span><span class="sxs-lookup"><span data-stu-id="47f92-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="47f92-104">يتم أيضا تسجيل معلومات العميل.</span><span class="sxs-lookup"><span data-stu-id="47f92-104">The client information is also logged.</span></span> <span data-ttu-id="47f92-105">فيما يلي كيفية تحديد عنوان IP:</span><span class="sxs-lookup"><span data-stu-id="47f92-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="47f92-106">انتقل إلى مركز التوافق في [Office 365 &.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="47f92-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="47f92-107">حدد **البحث في** سجل تدقيق  >  **[البحث.](https://go.microsoft.com/fwlink/?linkid=2103759)**</span><span class="sxs-lookup"><span data-stu-id="47f92-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="47f92-108">إذا رأيت إشعارا بأنه يجب تشغيل التدقيق، فمضي قدما وقلبه الآن.</span><span class="sxs-lookup"><span data-stu-id="47f92-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="47f92-109">إذا لم يتم تمكين هذه الميزة، فلن تتمكن نتائج البحث من سحب البيانات من التواريخ السابقة.</span><span class="sxs-lookup"><span data-stu-id="47f92-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="47f92-110">إذا كنت مهتما بنشاط معين، فحدده من **قائمة الأنشطة؛** وإلا، سيتم إرجاع كل الأنشطة للمستخدم المحدد بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="47f92-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="47f92-111">تجدر الإشارة إلى أن بعض الأنشطة قد لا تكون متوفرة للاختيار من قائمة **"الأنشطة"؛** ومع ذلك، سيتم إرجاع عناصر التدقيق هذه إذا تم تحديد "إظهار النتائج **لكل** الأنشطة" (الإعداد الافتراضي).</span><span class="sxs-lookup"><span data-stu-id="47f92-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="47f92-112">حدد نطاق التاريخ، وفي **حقل** "المستخدمون"، حدد اسم المستخدم للمستخدم الذي تريد التحقق منه.</span><span class="sxs-lookup"><span data-stu-id="47f92-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="47f92-113">حدد **"بحث".**</span><span class="sxs-lookup"><span data-stu-id="47f92-113">Select **Search**.</span></span> <span data-ttu-id="47f92-114">تظهر الأنشطة ضمن **"النتائج".**</span><span class="sxs-lookup"><span data-stu-id="47f92-114">The activities appear under **Results**.</span></span> <span data-ttu-id="47f92-115">يمكنك الاطلاع على عنوان IP لكل نشاط.</span><span class="sxs-lookup"><span data-stu-id="47f92-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="47f92-116">لعرض التفاصيل، حدد نشاطا، ثم حدد **"مزيد من المعلومات".**</span><span class="sxs-lookup"><span data-stu-id="47f92-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="47f92-117">لمعرفة المزيد، راجع البحث في سجل تدقيق Office 365 استكشاف الأخطاء [وإصلاحها في السيناريوهات الشائعة.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="47f92-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>