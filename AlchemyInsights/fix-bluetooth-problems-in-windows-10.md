---
title: إصلاح مشاكل Bluetooth في Windows 10
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
- "9001475"
- "3506"
ms.openlocfilehash: 7e7a397a1f6777972a81bcbb6bffa1c98d8370a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730146"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="db102-102">إصلاح مشاكل Bluetooth في Windows 10</span><span class="sxs-lookup"><span data-stu-id="db102-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="db102-103">إذا كانت أيقونه Bluetooth مفقوده أو لا يمكن تشغيل Bluetooth أو تشغيلها ، فقد تحتاج إلى تشغيل مستكشف أخطاء Bluetooth وإصلاحها.</span><span class="sxs-lookup"><span data-stu-id="db102-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="db102-104">[افتح إعدادات استكشاف الأخطاء وإصلاحها](ms-settings:troubleshoot)، وانقر فوق **Bluetooth** ضمن **البحث عن المشاكل الأخرى وإصلاحها**، انقر فوق **تشغيل مستكشف الأخطاء ومصلحها**.</span><span class="sxs-lookup"><span data-stu-id="db102-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="db102-105">إذا لم تتمكن من رؤية أيقونه Bluetooth ، ولكن ظهر Bluetooth في أداره الجهاز:</span><span class="sxs-lookup"><span data-stu-id="db102-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="db102-106">في أداره الاجهزه ، انقر فوق **Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="db102-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="db102-107">اضغط باستمرار (أو انقر بزر الماوس الأيمن) علي اسم محول Bluetooth ثم انقر فوق **أزاله تثبيت الجهاز**.</span><span class="sxs-lookup"><span data-stu-id="db102-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="db102-108">قم بإيقاف تشغيل جهاز Windows ، وانتظر بضع ثوان ، ثم أعد تشغيله.</span><span class="sxs-lookup"><span data-stu-id="db102-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="db102-109">سيحاول Windows أعاده تثبيت برنامج التشغيل.</span><span class="sxs-lookup"><span data-stu-id="db102-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="db102-110">إذا قمت مؤخرا بتثبيت تحديثات Windows 10 أو ترقيتها إلى Windows 10 ، فقد ترغب في التحقق من تحديثات برنامج التشغيل:</span><span class="sxs-lookup"><span data-stu-id="db102-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="db102-111">في أداره الاجهزه ، انقر فوق **Bluetooth**، ثم انقر فوق اسم محول Bluetooth (الذي قد يتضمن الكلمة "راديو").</span><span class="sxs-lookup"><span data-stu-id="db102-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="db102-112">اضغط باستمرار (أو انقر بزر الماوس الأيمن) فوق محول Bluetooth ، ثم انقر فوق **تحديث**  >  **البحث تلقائيا عن برنامج تشغيل محدث**.</span><span class="sxs-lookup"><span data-stu-id="db102-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="db102-113">اتبع الخطوات ، ثم انقر فوق **إغلاق**.</span><span class="sxs-lookup"><span data-stu-id="db102-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="db102-114">إذا تعذر علي Windows العثور علي برنامج تشغيل Bluetooth جديد ، فيمكنك زيارة موقع ويب الخاص بالشركة المصنعة للكمبيوتر الشخصي وتنزيل أحدث برنامج تشغيل Bluetooth من هناك.</span><span class="sxs-lookup"><span data-stu-id="db102-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="db102-115">بعد تنزيله ، انقر فوق **تحديث برنامج**  >  **التشغيل استعرض الكمبيوتر للحصول علي برنامج التشغيل**،  >  **واستعرض وصولا** إلى الموقع حيث يتم تخزين ملفات برنامج التشغيل > **موافق**  >  **Next**، واتبع الخطوات التي يجب تثبيتها.</span><span class="sxs-lookup"><span data-stu-id="db102-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="db102-116">بعد تثبيت برنامج التشغيل المحدث ، أعد تشغيل الجهاز ، وتحقق مما إذا كان ذلك يقوم بإصلاح مشكله الاتصال.</span><span class="sxs-lookup"><span data-stu-id="db102-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="db102-117">للحصول علي مزيد من التفاصيل حول كيفيه استكشاف أخطاء Bluetooth وإصلاحها ، يرجى مراجعه المقالة الكاملة ، [إصلاح مشاكل Bluetooth في Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span><span class="sxs-lookup"><span data-stu-id="db102-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
