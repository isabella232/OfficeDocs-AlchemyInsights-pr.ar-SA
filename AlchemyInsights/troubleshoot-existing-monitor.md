---
title: استكشاف أخطاء جهاز العرض الموجود
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690698"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="8575a-102">استكشاف أخطاء جهاز عرض موجود وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="8575a-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="8575a-103">جرب هذه الحلول لاستكشاف الأخطاء وإصلاحها.</span><span class="sxs-lookup"><span data-stu-id="8575a-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="8575a-104">**تحديث شاشه العرض الخاصة بك:**</span><span class="sxs-lookup"><span data-stu-id="8575a-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="8575a-105">اضغط علي المفاتيح التالية في الوقت نفسه: مفتاح Windows + Ctrl + Shift + B. سيؤدي ذلك إلى تحديث الاتصالات ببرنامج تشغيل الرسومات.</span><span class="sxs-lookup"><span data-stu-id="8575a-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="8575a-106">ستومض أجهزه العرض الخاصة بك قريبا وتعود بعد قليل من الثواني.</span><span class="sxs-lookup"><span data-stu-id="8575a-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="8575a-107">**استكشاف أخطاء جهاز العرض وإصلاحها:**</span><span class="sxs-lookup"><span data-stu-id="8575a-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="8575a-108">قم بإلغاء توصيل الكبل الذي يصل الكمبيوتر بجهاز العرض ، وقم بتوصيله مره أخرى.</span><span class="sxs-lookup"><span data-stu-id="8575a-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="8575a-109">اقطع اتصال اي أجهزه غير ضرورية من الكمبيوتر الشخصي (مثل المحولات أو المساحات).</span><span class="sxs-lookup"><span data-stu-id="8575a-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="8575a-110">**إذا قمت مؤخرا بتثبيت تحديث علي الكمبيوتر الشخصي ، فيمكنك استرجاع برنامج تشغيل العرض الخاص بك:**</span><span class="sxs-lookup"><span data-stu-id="8575a-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="8575a-111">حدد **أبدا**، واكتب **أداره الاجهزه**، وحدد **أداره الاجهزه** من النتائج.</span><span class="sxs-lookup"><span data-stu-id="8575a-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="8575a-112">قم بتوسيع المقطع **محولات العرض** ، وانقر بزر الماوس الأيمن فوق محول العرض ، **وحدد أندس**.</span><span class="sxs-lookup"><span data-stu-id="8575a-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="8575a-113">انتقل إلى علامة التبويب **برنامج التشغيل** وحدد **استعاده برنامج التشغيل السابق**.</span><span class="sxs-lookup"><span data-stu-id="8575a-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="8575a-114">ملاحظه: إذا لم يكن هذا الخيار متوفرا أو إذا كان باللون الرمادي ، فحدد " **لا** " من القائمة أدناه للانتقال إلى الخطوة التالية.</span><span class="sxs-lookup"><span data-stu-id="8575a-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="8575a-115">قد تحتاج إلى أعاده تشغيل الكمبيوتر قبل ان تصبح هذه التغييرات ساريه المفعول.</span><span class="sxs-lookup"><span data-stu-id="8575a-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="8575a-116">**إلغاء تثبيت برنامج تشغيل العرض وأعاده تثبيته:**</span><span class="sxs-lookup"><span data-stu-id="8575a-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="8575a-117">حدد **أبدا**، واكتب **أداره الاجهزه**، وحدد **أداره الاجهزه** من النتائج.</span><span class="sxs-lookup"><span data-stu-id="8575a-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="8575a-118">قم بتوسيع المقطع **محولات العرض** ، وانقر بزر الماوس الأيمن فوق محول العرض ، أندس حدد **أزاله التثبيت**.</span><span class="sxs-lookup"><span data-stu-id="8575a-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="8575a-119">حدد المربع الموجود إلى جانب **حذف برنامج التشغيل لهذا الجهاز** وحدد **أزاله التثبيت**.</span><span class="sxs-lookup"><span data-stu-id="8575a-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="8575a-120">ملاحظه: قد تتم مطالبتك باعاده تشغيل الكمبيوتر في هذه المرحلة.</span><span class="sxs-lookup"><span data-stu-id="8575a-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="8575a-121">تاكد من كتابه الإرشادات المتبقية قبل أعاده التشغيل.</span><span class="sxs-lookup"><span data-stu-id="8575a-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="8575a-122">افتح Device Manager مره أخرى.</span><span class="sxs-lookup"><span data-stu-id="8575a-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="8575a-123">قم بتوسيع المقطع **محولات العرض** ، وانقر بزر الماوس الأيمن فوق محول العرض ، وحدد **تحديث برنامج التشغيل**.</span><span class="sxs-lookup"><span data-stu-id="8575a-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="8575a-124">حدد **البحث تلقائيا عن برنامج تشغيل التحديث** واتبع إرشادات التثبيت.</span><span class="sxs-lookup"><span data-stu-id="8575a-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>