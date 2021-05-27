---
title: مخزون البرامج مفقود أو غير دقيق
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676049"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a><span data-ttu-id="afba1-102">مخزون البرامج مفقود أو غير دقيق</span><span class="sxs-lookup"><span data-stu-id="afba1-102">Software inventory is missing or inaccurate</span></span>

<span data-ttu-id="afba1-103">إن مخزون البرامج في إدارة المخاطر والثغرات الأمنية (TVM) هو قائمة البرامج المعروفة في مؤسستك باستخدام تعدادات النظام الأساسي الشائع (CPE) الرسمية.</span><span class="sxs-lookup"><span data-stu-id="afba1-103">The software inventory in threat and vulnerability management (TVM) is a list of known software in your organization with official Common Platform Enumerations (CPE).</span></span>

<span data-ttu-id="afba1-104">لا يتم نشر نقاط الضعف في منتجات البرامج التي لا تملك CPE رسمية.</span><span class="sxs-lookup"><span data-stu-id="afba1-104">Software products without an official CPE don’t have vulnerabilities published.</span></span> <span data-ttu-id="afba1-105">يتضمن المخزون أيضا تفاصيل مثل اسم المورد وعدد نقاط الضعف والتهديدات وعدد الأجهزة التي يتم عرضها.</span><span class="sxs-lookup"><span data-stu-id="afba1-105">The inventory also includes details such as the name of the vendor, number of weaknesses, threats, and number of exposed devices.</span></span>

<span data-ttu-id="afba1-106">تنعكس تغييرات البرامج على الأجهزة عادة في مداخل الأمان في غضون ساعتين.</span><span class="sxs-lookup"><span data-stu-id="afba1-106">Software changes on devices are typically reflected in security portals within two hours.</span></span> <span data-ttu-id="afba1-107">ومع ذلك، قد يستغرق الأمر في بعض الأحيان وقتا أطول.</span><span class="sxs-lookup"><span data-stu-id="afba1-107">However, it may sometimes take longer.</span></span> <span data-ttu-id="afba1-108">لا توجد حاليا أي طريقة فرض المزامنة؛ هذا تقييم مستمر مستمر.</span><span class="sxs-lookup"><span data-stu-id="afba1-108">There’s currently no way to force a sync; this is an ongoing continuous assessment.</span></span>

<span data-ttu-id="afba1-109">إذا قمت بتغيير البرنامج ولم يظهر التغيير بدقة في TVM بعد مرور 5 ساعات، فاتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="afba1-109">If you made a software change and the change is not accurately reflected in TVM after 5 hours, follow these steps:</span></span>

1. <span data-ttu-id="afba1-110">تحقق من قسم دليل البرنامج لفهم كيفية اكتشاف البرنامج.</span><span class="sxs-lookup"><span data-stu-id="afba1-110">Check the software evidence section to understand how the software was detected.</span></span>
1. <span data-ttu-id="afba1-111">تأكد من دعم البرنامج.</span><span class="sxs-lookup"><span data-stu-id="afba1-111">Make sure that the software is supported.</span></span> <span data-ttu-id="afba1-112">قد يكون البرنامج مرئيا فقط على مستوى الجهاز حتى لو لم يكن مدعوما حاليا من قبل إدارة المخاطر والثغرات الأمنية.</span><span class="sxs-lookup"><span data-stu-id="afba1-112">Software may be visible only at the device level even if it is currently not supported by threat and vulnerability management.</span></span> <span data-ttu-id="afba1-113">ومع ذلك، لا تتوفر سوى بيانات محدودة.</span><span class="sxs-lookup"><span data-stu-id="afba1-113">However, only limited data is available.</span></span>
1. <span data-ttu-id="afba1-114">للحصول على خطوات الإبلاغ عن عدم الدقة من المدخل، راجع [الإبلاغ عن عدم الدقة](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span><span class="sxs-lookup"><span data-stu-id="afba1-114">For steps to report the inaccuracy from the portal, see [Report inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span></span>
   
    <span data-ttu-id="afba1-115">**ملاحظة:** الإبلاغ عن عدم دقة من مدخل MDE هو قناة ذات طريقة واحدة إلى الهندسة.</span><span class="sxs-lookup"><span data-stu-id="afba1-115">**Note**: Reporting an inaccuracy from the MDE portal is a one-way channel to engineering.</span></span> <span data-ttu-id="afba1-116">إذا كانت المشكلة عاجلة، فافتح تذكرة دعم.</span><span class="sxs-lookup"><span data-stu-id="afba1-116">If the issue is urgent, open a support ticket.</span></span>

<span data-ttu-id="afba1-117">لمزيد من المعلومات، راجع [مخزون البرامج - إدارة المخاطر والثغرات الأمنية](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span><span class="sxs-lookup"><span data-stu-id="afba1-117">For more information, see [Software inventory - threat and vulnerability management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span></span>