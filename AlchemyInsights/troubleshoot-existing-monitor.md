---
title: استكشاف الأخطاء في جهاز العرض الموجود وإصلاحها
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824566"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="30017-102">استكشاف الأخطاء في جهاز عرض موجود وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="30017-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="30017-103">جرب هذه الحلول لا استكشاف الأخطاء في جهاز العرض وإصلاحها.</span><span class="sxs-lookup"><span data-stu-id="30017-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="30017-104">**تحديث عرض جهاز العرض:**</span><span class="sxs-lookup"><span data-stu-id="30017-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="30017-105">اضغط على المفاتيح التالية في الوقت نفسه: مفتاح Windows + Ctrl + Shift + B. سيتم تحديث الاتصال مع برنامج تشغيل الرسومات.</span><span class="sxs-lookup"><span data-stu-id="30017-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="30017-106">ستومض أجهزة العرض الخاصة بك بشكل لحظة وستعود بعد بضع ثوان.</span><span class="sxs-lookup"><span data-stu-id="30017-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="30017-107">**استكشاف الأخطاء في أجهزة جهاز العرض وإصلاحها:**</span><span class="sxs-lookup"><span data-stu-id="30017-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="30017-108">افصل الكبل الذي يصل جهاز الكمبيوتر الخاص بك بشاشة العرض، ثم قم بتوصيله مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="30017-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="30017-109">اقطع اتصال أي أجهزة غير ضرورية من الكمبيوتر الشخصي (مثل المحولات أو الإرساء).</span><span class="sxs-lookup"><span data-stu-id="30017-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="30017-110">**إذا قمت مؤخرا بتثبيت تحديث على الكمبيوتر الشخصي، يمكنك التراجع عن برنامج تشغيل جهاز العرض:**</span><span class="sxs-lookup"><span data-stu-id="30017-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="30017-111">حدد **بدء**، وا اكتب **إدارة الأجهزة**، وحدد إدارة **الأجهزة** من النتائج.</span><span class="sxs-lookup"><span data-stu-id="30017-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="30017-112">قم بتوسيع **المقطع محولات** العرض، وانقر بزر الماوس الأيمن فوق محول العرض، وحدد **خصائص**.</span><span class="sxs-lookup"><span data-stu-id="30017-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="30017-113">انتقل إلى علامة **التبويب برنامج التشغيل** وحدد التراجع عن برنامج **التشغيل**.</span><span class="sxs-lookup"><span data-stu-id="30017-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="30017-114">ملاحظة: إذا لم يكن هذا الخيار متوفرا أو كان رمادي اللون، فحدد **لا** من الخيارات أدناه للانتقال إلى الخطوة التالية.</span><span class="sxs-lookup"><span data-stu-id="30017-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="30017-115">قد تحتاج إلى إعادة تشغيل الكمبيوتر قبل أن يتم إدخال هذه التغييرات.</span><span class="sxs-lookup"><span data-stu-id="30017-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="30017-116">**إلغاء تثبيت برنامج تشغيل جهاز العرض وإعادة تثبيته:**</span><span class="sxs-lookup"><span data-stu-id="30017-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="30017-117">حدد **بدء**، وا اكتب **إدارة الأجهزة**، وحدد إدارة **الأجهزة** من النتائج.</span><span class="sxs-lookup"><span data-stu-id="30017-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="30017-118">قم بتوسيع **المقطع محولات** العرض، وانقر بزر الماوس الأيمن فوق محول العرض، وحدد **إلغاء تثبيت الجهاز**.</span><span class="sxs-lookup"><span data-stu-id="30017-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="30017-119">حدد المربع بجانب **حذف برنامج التشغيل لهذا الجهاز** وحدد إلغاء **التثبيت**.</span><span class="sxs-lookup"><span data-stu-id="30017-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="30017-120">ملاحظة: قد يطلب منك إعادة تشغيل الكمبيوتر في هذه المرحلة.</span><span class="sxs-lookup"><span data-stu-id="30017-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="30017-121">تأكد من كتابة الإرشادات المتبقية قبل إعادة التشغيل.</span><span class="sxs-lookup"><span data-stu-id="30017-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="30017-122">افتح إدارة الأجهزة مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="30017-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="30017-123">قم بتوسيع **المقطع محولات** العرض، وانقر بزر الماوس الأيمن فوق محول العرض، وحدد **تحديث برنامج التشغيل**.</span><span class="sxs-lookup"><span data-stu-id="30017-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="30017-124">حدد **البحث تلقائيا عن برنامج تشغيل التحديث واتبع** إرشادات التثبيت.</span><span class="sxs-lookup"><span data-stu-id="30017-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>