---
title: إصلاح مشاكل البلوتوث في Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001475"
- "3506"
ms.openlocfilehash: 94dda7a42632f57ce3aef5f467b87df1033b8d49
ms.sourcegitcommit: 9a35768444824cde9e192f1d9daafc9157437244
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/25/2020
ms.locfileid: "42268550"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="83da9-102">إصلاح مشاكل البلوتوث في Windows 10</span><span class="sxs-lookup"><span data-stu-id="83da9-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="83da9-103">إذا كان رمز Bluetooth مفقودًا أو تعذر تشغيل Bluetooth أو إيقاف تشغيله، فقد تحتاج إلى تشغيل مستكشف أخطاء Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="83da9-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="83da9-104">[فتح إعدادات استكشاف الأخطاء وإصلاحها](ms-settings:troubleshoot)، انقر فوق **بلوتوث** تحت **البحث وإصلاح المشاكل الأخرى**، انقر فوق تشغيل مستكشف الأخطاء **وإصلاحها**.</span><span class="sxs-lookup"><span data-stu-id="83da9-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="83da9-105">إذا كنت لا ترى رمز Bluetooth، ولكن يظهر Bluetooth في إدارة الأجهزة:</span><span class="sxs-lookup"><span data-stu-id="83da9-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="83da9-106">في إدارة الأجهزة، انقر فوق **Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="83da9-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="83da9-107">اضغط مع الاستمرار (أو انقر بزر الماوس الأيمن) على اسم محول Bluetooth وانقر فوق **إلغاء تثبيت الجهاز**.</span><span class="sxs-lookup"><span data-stu-id="83da9-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="83da9-108">قم بإيقاف تشغيل جهاز Windows، وانتظر بضع ثوانٍ، ثم أعد تشغيله.</span><span class="sxs-lookup"><span data-stu-id="83da9-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="83da9-109">سيحاول Windows إعادة تثبيت برنامج التشغيل.</span><span class="sxs-lookup"><span data-stu-id="83da9-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="83da9-110">إذا قمت مؤخرًا بتثبيت تحديثات Windows 10 أو تمت ترقيتها إلى Windows 10، فقد تحتاج إلى التحقق من تحديثات برنامج التشغيل:</span><span class="sxs-lookup"><span data-stu-id="83da9-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="83da9-111">في إدارة الأجهزة، انقر فوق **Bluetooth**، ثم انقر فوق اسم محول Bluetooth (الذي قد يتضمن كلمة "راديو").</span><span class="sxs-lookup"><span data-stu-id="83da9-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="83da9-112">اضغط مع الاستمرار (أو انقر بزر الماوس الأيمن) على محول Bluetooth، ثم انقر فوق **تحديث برنامج البحث** > **تلقائيًا عن برنامج التشغيل المحدث**.</span><span class="sxs-lookup"><span data-stu-id="83da9-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="83da9-113">اتبع الخطوات، ثم انقر فوق **إغلاق**.</span><span class="sxs-lookup"><span data-stu-id="83da9-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="83da9-114">إذا لم يتمكن Windows من العثور على برنامج تشغيل Bluetooth جديد، فقم بزيارة موقع ويب الشركة المصنعة للكمبيوتر الشخصي وتنزيل أحدث برنامج تشغيل Bluetooth من هناك.</span><span class="sxs-lookup"><span data-stu-id="83da9-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="83da9-115">بعد تنزيله، انقر فوق **تحديث برنامج تشغيل** > **استعراض جهاز الكمبيوتر الخاص بي لبرنامج التشغيل** > **استعراض** للموقع حيث يتم تخزين ملفات برنامج التشغيل > **موافق** > **التالي**، واتبع الخطوات لتثبيت.</span><span class="sxs-lookup"><span data-stu-id="83da9-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="83da9-116">بعد تثبيت برنامج التشغيل المحدث، أعد تشغيل الجهاز، ثم تحقق مما إذا كان ذلك يحل مشكلة الاتصال.</span><span class="sxs-lookup"><span data-stu-id="83da9-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="83da9-117">لمزيد من التفاصيل حول كيفية استكشاف مشاكل البلوتوث، يرجى الاطلاع على المقالة الكاملة، [إصلاح مشاكل البلوتوث في Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span><span class="sxs-lookup"><span data-stu-id="83da9-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
