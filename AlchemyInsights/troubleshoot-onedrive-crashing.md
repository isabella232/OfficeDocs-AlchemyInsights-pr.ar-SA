---
title: استكشاف أخطاء تعطل OneDrive وإصلاحها
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/15/2020
ms.locfileid: "44748703"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="51efa-102">استكشاف أخطاء تعطل OneDrive وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="51efa-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="51efa-103">إذا تعطل OneDrive بشكل متكرر، حاول تنفيذ الخطوات التالية لاستكشاف الأخطاء وإصلاحها:</span><span class="sxs-lookup"><span data-stu-id="51efa-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="51efa-104">**تأكد من عدم تعيين مفاتيح التسجيل:**</span><span class="sxs-lookup"><span data-stu-id="51efa-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="51efa-105">باستخدام محرر التسجيل، انتقل إلى HKEY_LOCAL_MACHINE\SOFTWARE\نُهج\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="51efa-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="51efa-106">إذا كان DisableFileSyncNGSC موجوداً وتعيين إلى 1، افتح المفتاح وتغيير القيمة إلى 0.</span><span class="sxs-lookup"><span data-stu-id="51efa-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="51efa-107">تشغيل OneDrive يدويًا عن طريق الانتقال إلى Start</span><span class="sxs-lookup"><span data-stu-id="51efa-107">Manually launch OneDrive by going to Start</span></span> ![اضغط على مفتاح Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="51efa-109">، اكتب أندريف في مربع البحث، ثم انقر فوق تطبيق سطح المكتب OneDrive.</span><span class="sxs-lookup"><span data-stu-id="51efa-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="51efa-110">**إعادة تعيين أندريف:**</span><span class="sxs-lookup"><span data-stu-id="51efa-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="51efa-111">تلاحظ:</span><span class="sxs-lookup"><span data-stu-id="51efa-111">Notes:</span></span>

- <span data-ttu-id="51efa-112">تؤدي إعادة تعيين OneDrive إلى قطع اتصال كافة اتصالات المزامنة الموجودة لديك (بما في ذلك OneDrive الخاص بك في حالة الإعداد).</span><span class="sxs-lookup"><span data-stu-id="51efa-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="51efa-113">لن تفقد الملفات أو البيانات عن طريق إعادة تعيين OneDrive على الكمبيوتر.</span><span class="sxs-lookup"><span data-stu-id="51efa-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="51efa-114">**لإعادة تعيين أندريف:**</span><span class="sxs-lookup"><span data-stu-id="51efa-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="51efa-115">افتح مربع حوار تشغيل بالضغط على مفتاح Windows و R.</span><span class="sxs-lookup"><span data-stu-id="51efa-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="51efa-116">اكتب %localappdata%\Microsoft\OneDrive\onedrive.exe /إعادة تعيين ثم اضغط موافق.</span><span class="sxs-lookup"><span data-stu-id="51efa-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="51efa-117">قد يظهر إطار أمر لفترة وجيزة.</span><span class="sxs-lookup"><span data-stu-id="51efa-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="51efa-118">تشغيل OneDrive يدويًا عن طريق الانتقال إلى Start</span><span class="sxs-lookup"><span data-stu-id="51efa-118">Manually launch OneDrive by going to Start</span></span> ![اضغط على مفتاح Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="51efa-120">، اكتب أندريف في مربع البحث، ثم انقر فوق تطبيق سطح المكتب OneDrive.</span><span class="sxs-lookup"><span data-stu-id="51efa-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="51efa-121">تلاحظ:</span><span class="sxs-lookup"><span data-stu-id="51efa-121">Notes:</span></span>

- <span data-ttu-id="51efa-122">إذا اخترت مزامنة بعض المجلدات فقط قبل إعادة التعيين، فستحتاج إلى القيام بذلك مرة أخرى بمجرد اكتمال المزامنة.</span><span class="sxs-lookup"><span data-stu-id="51efa-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="51efa-123">اقرأ [اختر المجلدات OneDrive التي تريد مزامنتها مع الكمبيوتر للحصول](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)على مزيد من   المعلومات.</span><span class="sxs-lookup"><span data-stu-id="51efa-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="51efa-124">ستحتاج إلى إكمال هذا لـ OneDrive وOneDrive الخاصين بك.</span><span class="sxs-lookup"><span data-stu-id="51efa-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>