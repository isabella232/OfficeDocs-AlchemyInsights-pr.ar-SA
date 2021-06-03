---
title: إنشاء علامات أو مجموعات الأجهزة وإدارتها
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731256"
---
# <a name="create-and-manage-device-tags-or-groups"></a><span data-ttu-id="2d7a3-102">إنشاء علامات أو مجموعات الأجهزة وإدارتها</span><span class="sxs-lookup"><span data-stu-id="2d7a3-102">Create and manage device tags or groups</span></span>

<span data-ttu-id="2d7a3-103">أضف علامات على الأجهزة لإنشاء انتماء مجموعة منطقي.</span><span class="sxs-lookup"><span data-stu-id="2d7a3-103">Add tags on devices to create a logical group affiliation.</span></span> <span data-ttu-id="2d7a3-104">تدعم علامات الجهاز التعيين المناسب للشبكة، مما يسمح لك بإرفاق علامات مختلفة لالتقاط السياق وتمكين إنشاء قائمة ديناميكية كجزء من حادث.</span><span class="sxs-lookup"><span data-stu-id="2d7a3-104">Device tags support proper mapping of the network, enabling you to attach different tags to capture context and to enable dynamic list creation as part of an incident.</span></span> <span data-ttu-id="2d7a3-105">يمكن استخدام العلامات كتصفية في طريقة عرض قائمة الأجهزة، أو لمجموعة الأجهزة.</span><span class="sxs-lookup"><span data-stu-id="2d7a3-105">Tags can be used as a filter in Devices list view, or to group devices.</span></span> <span data-ttu-id="2d7a3-106">لمزيد من المعلومات حول تجميع الأجهزة، راجع [إنشاء علامات الجهاز وإدارتها](/microsoft-365/security/defender-endpoint/machine-tags).</span><span class="sxs-lookup"><span data-stu-id="2d7a3-106">For more information on device grouping, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>

<span data-ttu-id="2d7a3-107">يمكنك إضافة العلامات على الأجهزة من خلال:</span><span class="sxs-lookup"><span data-stu-id="2d7a3-107">You can add tags on devices by:</span></span>

- <span data-ttu-id="2d7a3-108">استخدام المدخل</span><span class="sxs-lookup"><span data-stu-id="2d7a3-108">Using the portal</span></span>

- <span data-ttu-id="2d7a3-109">تعيين قيمة مفتاح تسجيل</span><span class="sxs-lookup"><span data-stu-id="2d7a3-109">Setting a registry key value</span></span>
 
<span data-ttu-id="2d7a3-110">**ملاحظة:** قد يكون هناك زمن بين وقت إضافة علامة إلى جهاز ومدى توفرها في قائمة الأجهزة وصفحة الجهاز.</span><span class="sxs-lookup"><span data-stu-id="2d7a3-110">**Note:** There could be latency between the time a tag is added to a device and its availability in the devices list and device page.</span></span>

<span data-ttu-id="2d7a3-111">لإضافة علامات الجهاز باستخدام API، راجع [إضافة API علامات](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags)الجهاز أو إزالتها .</span><span class="sxs-lookup"><span data-stu-id="2d7a3-111">To add device tags using API, see [Add or remove device tags API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span></span>

## <a name="add-and-manage-device-tags-using-the-portal"></a><span data-ttu-id="2d7a3-112">إضافة علامات الجهاز وإدارتها باستخدام المدخل</span><span class="sxs-lookup"><span data-stu-id="2d7a3-112">Add and manage device tags using the portal</span></span>

1. <span data-ttu-id="2d7a3-113">حدد الجهاز الذي تريد إدارة العلامات عليه.</span><span class="sxs-lookup"><span data-stu-id="2d7a3-113">Select the device that you want to manage tags on.</span></span> <span data-ttu-id="2d7a3-114">يمكنك تحديد جهاز أو البحث عنه من أي من طرق العرض التالية:</span><span class="sxs-lookup"><span data-stu-id="2d7a3-114">You can select or search for a device from any of the following views:</span></span>

    - <span data-ttu-id="2d7a3-115">**لوحة معلومات عمليات الأمان** حدد اسم الجهاز من القسم أهم الأجهزة التي بها تنبيهات نشطة.</span><span class="sxs-lookup"><span data-stu-id="2d7a3-115">**Security operations dashboard** Select the device name from the Top devices with active alerts section.</span></span>
    - <span data-ttu-id="2d7a3-116">**قائمة انتظار التنبيهات** - حدد اسم الجهاز إلى جانب أيقونة الجهاز من قائمة انتظار التنبيهات.</span><span class="sxs-lookup"><span data-stu-id="2d7a3-116">**Alerts queue** - Select the device name beside the device icon from the alerts queue.</span></span>
    - <span data-ttu-id="2d7a3-117">**قائمة الأجهزة** - حدد اسم الجهاز من قائمة الأجهزة.</span><span class="sxs-lookup"><span data-stu-id="2d7a3-117">**Devices list** - Select the device name from the list of devices.</span></span>
    - <span data-ttu-id="2d7a3-118">**مربع البحث** - حدد الجهاز من القائمة المنسدلة وأدخل اسم الجهاز.</span><span class="sxs-lookup"><span data-stu-id="2d7a3-118">**Search box** - Select Device from the drop-down menu and enter the device name.</span></span>

    <span data-ttu-id="2d7a3-119">يمكنك أيضا الوصول إلى صفحة التنبيه من خلال طريقتي عرض الملف وIP.</span><span class="sxs-lookup"><span data-stu-id="2d7a3-119">You can also get to the alert page through the file and IP views.</span></span>

1. <span data-ttu-id="2d7a3-120">حدد **إدارة العلامات** من صف إجراءات الاستجابة.</span><span class="sxs-lookup"><span data-stu-id="2d7a3-120">Select **Manage Tags** from the row of Response actions.</span></span>

1. <span data-ttu-id="2d7a3-121">اكتب للعثور على العلامات أو إنشائها.</span><span class="sxs-lookup"><span data-stu-id="2d7a3-121">Type to find or create tags.</span></span>

<span data-ttu-id="2d7a3-122">تضاف العلامات إلى طريقة عرض الجهاز وتنعكس على طريقة عرض قائمة الأجهزة.</span><span class="sxs-lookup"><span data-stu-id="2d7a3-122">Tags are added to the device view and are reflected on the Devices list view.</span></span> <span data-ttu-id="2d7a3-123">يمكنك بعد ذلك استخدام عامل تصفية العلامات لرؤية قائمة الأجهزة ذات الصلة.</span><span class="sxs-lookup"><span data-stu-id="2d7a3-123">You can then use the Tags filter to see the relevant list of devices.</span></span>

<span data-ttu-id="2d7a3-124">لمزيد من المعلومات، راجع [إنشاء علامات الجهاز وإدارتها](/microsoft-365/security/defender-endpoint/machine-tags).</span><span class="sxs-lookup"><span data-stu-id="2d7a3-124">For more information, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>