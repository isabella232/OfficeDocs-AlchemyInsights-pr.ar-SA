---
title: إصلاح مشاكل Bluetooth في Windows 10
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
- "9001475"
- "3506"
ms.openlocfilehash: f20bf4a642e019c7901e988a027e0220f0f1b07b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812919"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="6ec0e-102">إصلاح مشاكل Bluetooth في Windows 10</span><span class="sxs-lookup"><span data-stu-id="6ec0e-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="6ec0e-103">إذا كانت أيقونة Bluetooth مفقودة أو لا يمكن تشغيل Bluetooth أو إيقاف تشغيله، فقد تحتاج إلى تشغيل م استكشاف مشاكل Bluetooth ومشكلاتها.</span><span class="sxs-lookup"><span data-stu-id="6ec0e-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="6ec0e-104">[افتح إعدادات استكشاف](ms-settings:troubleshoot)الأخطاء وإصلاحها، وانقر فوق **Bluetooth** ضمن البحث عن المشاكل الأخرى وإصلاحها، **وانقر** فوق **تشغيل مصلح الأخطاء ومصلحها**.</span><span class="sxs-lookup"><span data-stu-id="6ec0e-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="6ec0e-105">إذا لم تظهر أيقونة Bluetooth، ولكن يظهر Bluetooth في إدارة الأجهزة:</span><span class="sxs-lookup"><span data-stu-id="6ec0e-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="6ec0e-106">في إدارة الأجهزة، انقر فوق **Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="6ec0e-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="6ec0e-107">اضغط مع الاستمرار (أو انقر بزر الماوس الأيمن) على اسم محول Bluetooth وانقر فوق **إلغاء تثبيت الجهاز**.</span><span class="sxs-lookup"><span data-stu-id="6ec0e-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="6ec0e-108">قم بإيقاف تشغيل جهاز Windows، وانتظر بضع ثوان، ثم قم بإيقافه مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="6ec0e-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="6ec0e-109">سيحاول Windows إعادة تثبيت برنامج التشغيل.</span><span class="sxs-lookup"><span data-stu-id="6ec0e-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="6ec0e-110">إذا قمت مؤخرا بتثبيت تحديثات Windows 10 أو قمت بالترقية إلى Windows 10، فقد تحتاج إلى التحقق من وجود تحديثات برامج التشغيل:</span><span class="sxs-lookup"><span data-stu-id="6ec0e-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="6ec0e-111">في إدارة الأجهزة، انقر فوق **Bluetooth**، ثم انقر فوق اسم محول Bluetooth (الذي قد يتضمن الكلمة "radio").</span><span class="sxs-lookup"><span data-stu-id="6ec0e-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="6ec0e-112">اضغط باستمرار (أو انقر بزر الماوس الأيمن) على محول Bluetooth، ثم انقر فوق تحديث برنامج **التشغيل**  >  **البحث تلقائيا عن برنامج تشغيل محدث**.</span><span class="sxs-lookup"><span data-stu-id="6ec0e-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="6ec0e-113">اتبع الخطوات، ثم انقر فوق **إغلاق**.</span><span class="sxs-lookup"><span data-stu-id="6ec0e-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="6ec0e-114">إذا لم يعثر Windows على برنامج تشغيل Bluetooth جديد، يمكنك زيارة موقع الشركة المصنعة للكمبيوتر الشخصي على الويب وتنزيل أحدث برنامج تشغيل Bluetooth من هناك.</span><span class="sxs-lookup"><span data-stu-id="6ec0e-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="6ec0e-115">بعد تنزيله، انقر فوق تحديث برنامج **التشغيل** استعراض الكمبيوتر بحثا عن برنامج التشغيل استعرض بحثا عن الموقع حيث يتم تخزين ملفات برنامج التشغيل > موافق التالي ، واتبع خطوات  >    >     >  التثبيت.</span><span class="sxs-lookup"><span data-stu-id="6ec0e-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="6ec0e-116">بعد تثبيت برنامج التشغيل المحدث، أعد تشغيل الجهاز، ثم تحقق مما إذا كان ذلك قد أصلح مشكلة الاتصال.</span><span class="sxs-lookup"><span data-stu-id="6ec0e-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="6ec0e-117">لمزيد من التفاصيل حول كيفية استكشاف مشاكل Bluetooth وإصلاحها، الرجاء الاطلاع على المقالة الكاملة، إصلاح مشاكل [Bluetooth في Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span><span class="sxs-lookup"><span data-stu-id="6ec0e-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
