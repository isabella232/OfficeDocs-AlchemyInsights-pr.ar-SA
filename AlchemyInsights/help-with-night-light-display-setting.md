---
title: تعليمات حول إعداد عرض الضوء الليلي
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
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404137"
---
# <a name="help-with-the-night-light-display-setting"></a><span data-ttu-id="bd60e-102">تعليمات حول إعداد عرض الضوء الليلي</span><span class="sxs-lookup"><span data-stu-id="bd60e-102">Help with the night light display setting</span></span>

<span data-ttu-id="bd60e-103">لمعرفة المزيد حول إعدادات عرض الوقت الليلي، راجع تعيين العرض [للوقت الليلي في Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span><span class="sxs-lookup"><span data-stu-id="bd60e-103">To learn more about night time display settings, see [Set your display for night time in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span></span>

<span data-ttu-id="bd60e-104">إذا كانت خيارات الضوء الليلي باللون الرمادي في الإعدادات، فتحقق من برنامج تشغيل العرض:</span><span class="sxs-lookup"><span data-stu-id="bd60e-104">If the night light options are grayed out in Settings, check your display driver:</span></span> 

1. <span data-ttu-id="bd60e-105">انقر فوق مربع البحث على شريط المهام وا اكتب **إدارة الأجهزة**، ثم حدد **إدارة الأجهزة** في نتائج البحث.</span><span class="sxs-lookup"><span data-stu-id="bd60e-105">Click the search box on your taskbar and type **Device Manager**, and then select **Device Manager** in the search results.</span></span>
1. <span data-ttu-id="bd60e-106">توسيع **محولات العرض**.</span><span class="sxs-lookup"><span data-stu-id="bd60e-106">Expand **Display adapters**.</span></span> 

<span data-ttu-id="bd60e-107">لسوء الحظ، لا تتوفر ميزة الضوء الليلي إذا كان جهازك يستخدم برنامج تشغيل DisplayLink أو برنامج تشغيل عرض أساسي.</span><span class="sxs-lookup"><span data-stu-id="bd60e-107">Unfortunately, the night light feature is not available if your device uses a DisplayLink driver or a Basic Display driver.</span></span>

<span data-ttu-id="bd60e-108">تستخدم ميزة الضوء الليلي تقنية الرسومات الحديثة، لذلك قد تحتاج إلى تحديث برنامج تشغيل العرض:</span><span class="sxs-lookup"><span data-stu-id="bd60e-108">The night light feature makes use of recent graphics technology, so you might need to update your display driver:</span></span>  

- <span data-ttu-id="bd60e-109">تحقق من وجود تحديثات عن طريق الذهاب إلى **بدء** تحديث الإعدادات  >    >  **&**  >  **Windows Update** الأمان التحقق من وجود  >  **تحديثات**.</span><span class="sxs-lookup"><span data-stu-id="bd60e-109">Check for updates by going to **Start** > **Settings** > **Update & Security** > **Windows Update** > **Check for Updates**.</span></span>  

<span data-ttu-id="bd60e-110">OR</span><span class="sxs-lookup"><span data-stu-id="bd60e-110">OR</span></span>

- <span data-ttu-id="bd60e-111">تفضل بزيارة موقع ويب دعم الشركة المصنعة للأجهزة لتنزيل أحدث برامج تشغيل العرض وتثبيتها يدويا.</span><span class="sxs-lookup"><span data-stu-id="bd60e-111">Visit your hardware manufacturer's support website to manually download and install the latest display drivers.</span></span>

## <a name="reset-night-light-in-the-registry"></a><span data-ttu-id="bd60e-112">إعادة تعيين الضوء الليلي في السجل</span><span class="sxs-lookup"><span data-stu-id="bd60e-112">Reset night light in the registry</span></span>

<span data-ttu-id="bd60e-113">إذا لم ينجح تحديث برنامج تشغيل جهاز العرض، فقد تحتاج إلى إعادة تعيين الضوء الليلي في السجل.</span><span class="sxs-lookup"><span data-stu-id="bd60e-113">If updating your display driver didn't work, you might need to reset night light in the registry.</span></span>  

<span data-ttu-id="bd60e-114">**تنبيه:** يوصى بإجراء خطوة استكشاف الأخطاء وإصلاحها هذه للمستخدمين المتقدمين فقط.</span><span class="sxs-lookup"><span data-stu-id="bd60e-114">**Caution:** This troubleshooting step is recommended only for advanced users.</span></span> <span data-ttu-id="bd60e-115">قد تحدث مشاكل خطيرة إذا قمت بتعديل السجل بشكل غير صحيح.</span><span class="sxs-lookup"><span data-stu-id="bd60e-115">Serious problems can occur if you modify the registry incorrectly.</span></span> <span data-ttu-id="bd60e-116">لمزيد من الحماية، قم ب إنشاء سجل قبل تعديله حتى تتمكن من استعادته في حالة حدوث مشاكل.</span><span class="sxs-lookup"><span data-stu-id="bd60e-116">For added protection, back up the registry before you modify it so  you can restore it if problems occur.</span></span>

1. <span data-ttu-id="bd60e-117">في مربع البحث، اكتب **regedit**، ثم حدد **محرر السجل** في نتائج البحث.</span><span class="sxs-lookup"><span data-stu-id="bd60e-117">In the search box, type **regedit**, and then select **Registry Editor** in the search results.</span></span>

1. <span data-ttu-id="bd60e-118">انتقل إلى مفتاح التسجيل التالي:</span><span class="sxs-lookup"><span data-stu-id="bd60e-118">Go to the following registry key:</span></span> 

    <span data-ttu-id="bd60e-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span><span class="sxs-lookup"><span data-stu-id="bd60e-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span></span>

1. <span data-ttu-id="bd60e-120">تصدير المفتاح الفرعي التالي ثم حذفه:$$windows.data.bluelightreduction.bluelightreductionstate</span><span class="sxs-lookup"><span data-stu-id="bd60e-120">Export and then delete the following subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span></span>

1. <span data-ttu-id="bd60e-121">تصدير المفتاح الفرعي التالي ثم حذفه:$$windows.data.bluelightreduction.settings</span><span class="sxs-lookup"><span data-stu-id="bd60e-121">Export and then delete the following subkey:$$windows.data.bluelightreduction.settings</span></span>

1. <span data-ttu-id="bd60e-122">أعد تشغيل Windows وتحقق مما إذا كانت خيارات الضوء الليلي متوفرة.</span><span class="sxs-lookup"><span data-stu-id="bd60e-122">Restart Windows and verify if the night light options are available.</span></span>


