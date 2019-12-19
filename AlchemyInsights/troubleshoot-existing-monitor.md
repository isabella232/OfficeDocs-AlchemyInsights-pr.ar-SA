---
title: استكشاف أخطاء جهاز العرض الموجود
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: d90baddd01bdf8508bd6289509c8399b8241887a
ms.sourcegitcommit: 42463e8d8869f36225a27388d83d37629c6b149e
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/18/2019
ms.locfileid: "40738556"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="003ab-102">استكشاف أخطاء جهاز عرض موجود وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="003ab-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="003ab-103">جرب هذه الحلول لاستكشاف أخطاء جهاز العرض وإصلاحها.</span><span class="sxs-lookup"><span data-stu-id="003ab-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="003ab-104">**تحديث شاشه العرض:**</span><span class="sxs-lookup"><span data-stu-id="003ab-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="003ab-105">اضغط علي المفاتيح التالية في نفس الوقت: مفتاح Windows + Ctrl + Shift + B. سيؤدي هذا إلى تحديث الاتصال مع برنامج تشغيل الرسومات.</span><span class="sxs-lookup"><span data-stu-id="003ab-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="003ab-106">سيومض المراقبون للحظات ويعودون بعد بضع ثوان.</span><span class="sxs-lookup"><span data-stu-id="003ab-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="003ab-107">**استكشاف أخطاء أجهزه جهاز العرض وإصلاحها:**</span><span class="sxs-lookup"><span data-stu-id="003ab-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="003ab-108">افصل الكبل الذي يربط جهاز الكمبيوتر الخاص بك بجهاز العرض ، وقم بتوصيله مره أخرى.</span><span class="sxs-lookup"><span data-stu-id="003ab-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="003ab-109">افصل اي أجهزه غير أساسيه من جهاز الكمبيوتر الخاص بك (مثل المحولات أو الارصفه).</span><span class="sxs-lookup"><span data-stu-id="003ab-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="003ab-110">**إذا قمت مؤخرا بتثبيت تحديث علي جهاز الكمبيوتر الخاص بك ، يمكنك استرجاع برنامج تشغيل جهاز العرض:**</span><span class="sxs-lookup"><span data-stu-id="003ab-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="003ab-111">حدد **أبدا**، واكتب **أداره الاجهزه**، وحدد **أداره الاجهزه** من النتائج.</span><span class="sxs-lookup"><span data-stu-id="003ab-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="003ab-112">قم بتوسيع المقطع **محولات العرض** ، انقر بزر الماوس الأيمن فوق محول جهاز العرض ، الصولجانات حدد **خصائص**.</span><span class="sxs-lookup"><span data-stu-id="003ab-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="003ab-113">انتقل إلى علامة التبويب **برنامج التشغيل** وحدد استعاده **برنامج التشغيل**.</span><span class="sxs-lookup"><span data-stu-id="003ab-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="003ab-114">ملاحظه: إذا لم يكن هذا متوفرا أو تمت الاشاره اليه بالرمادي ، فحدد **لا** من الخيارات أدناه للانتقال إلى الخطوة التالية.</span><span class="sxs-lookup"><span data-stu-id="003ab-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="003ab-115">قد تحتاج إلى أعاده تشغيل جهاز الكمبيوتر الخاص بك قبل ان تسري هذه التغييرات.</span><span class="sxs-lookup"><span data-stu-id="003ab-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="003ab-116">**إلغاء تثبيت برنامج تشغيل العرض وأعاده تثبيته:**</span><span class="sxs-lookup"><span data-stu-id="003ab-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="003ab-117">حدد **أبدا**، واكتب **أداره الاجهزه**، وحدد **أداره الاجهزه** من النتائج.</span><span class="sxs-lookup"><span data-stu-id="003ab-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="003ab-118">قم بتوسيع المقطع **محولات العرض** انقر بزر الماوس الأيمن فوق محول جهاز العرض الخاص بك حدد **أزاله تثبيت الاجهزه**.</span><span class="sxs-lookup"><span data-stu-id="003ab-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="003ab-119">حدد المربع المجاور **لحذف برنامج التشغيل لهذا الجهاز** وحدد **إلغاء التثبيت**.</span><span class="sxs-lookup"><span data-stu-id="003ab-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="003ab-120">ملاحظه: قد يطلب منك أعاده تشغيل جهاز الكمبيوتر الخاص بك في هذه المرحلة.</span><span class="sxs-lookup"><span data-stu-id="003ab-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="003ab-121">تاكد من كتابه الإرشادات المتبقية قبل أعاده التشغيل.</span><span class="sxs-lookup"><span data-stu-id="003ab-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="003ab-122">افتح "أداره الاجهزه" مره أخرى.</span><span class="sxs-lookup"><span data-stu-id="003ab-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="003ab-123">قم بتوسيع المقطع **محولات العرض** انقر بزر الماوس الأيمن فوق محول جهاز العرض ثم حدد **تحديث برنامج التشغيل**.</span><span class="sxs-lookup"><span data-stu-id="003ab-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="003ab-124">حدد **البحث تلقائيا لتحديث برنامج التشغيل** واتبع إرشادات التثبيت.</span><span class="sxs-lookup"><span data-stu-id="003ab-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>