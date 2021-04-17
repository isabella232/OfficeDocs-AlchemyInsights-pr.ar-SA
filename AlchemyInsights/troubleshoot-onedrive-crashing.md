---
title: استكشاف أعطل OneDrive وإصلاحها
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
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826186"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="3827c-102">استكشاف أعطل OneDrive وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="3827c-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="3827c-103">إذا تعطل OneDrive بشكل متكرر، فجرب خطوات استكشاف الأخطاء وإصلاحها التالية:</span><span class="sxs-lookup"><span data-stu-id="3827c-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="3827c-104">**تأكد من عدم تعيين مفاتيح التسجيل:**</span><span class="sxs-lookup"><span data-stu-id="3827c-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="3827c-105">باستخدام محرر السجل، انتقل إلى HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="3827c-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="3827c-106">إذا كان DisableFileSyncNGSC موجودا وحدد إلى 1، فافتح المفتاح ثم غير القيمة إلى 0.</span><span class="sxs-lookup"><span data-stu-id="3827c-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="3827c-107">تشغيل OneDrive يدويا عن طريق الذهاب إلى البدء</span><span class="sxs-lookup"><span data-stu-id="3827c-107">Manually launch OneDrive by going to Start</span></span> ![اضغط على مفتاح Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="3827c-109">، اكتب OneDrive في مربع البحث، ثم انقر فوق تطبيق OneDrive لسطح المكتب.</span><span class="sxs-lookup"><span data-stu-id="3827c-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="3827c-110">**إعادة تعيين OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="3827c-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="3827c-111">ملاحظات:</span><span class="sxs-lookup"><span data-stu-id="3827c-111">Notes:</span></span>

- <span data-ttu-id="3827c-112">تفصل إعادة تعيين OneDrive كل اتصالات المزامنة الموجودة لديك (بما في ذلك OneDrive الشخصي في حالة إعداده).</span><span class="sxs-lookup"><span data-stu-id="3827c-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="3827c-113">لن تفقد الملفات أو البيانات عن طريق إعادة تعيين OneDrive على الكمبيوتر.</span><span class="sxs-lookup"><span data-stu-id="3827c-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="3827c-114">**لإعادة تعيين OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="3827c-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="3827c-115">افتح مربع الحوار تشغيل بالضغط على مفتاح Windows وR.</span><span class="sxs-lookup"><span data-stu-id="3827c-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="3827c-116">اكتب ٪localappdata٪\Microsoft\OneDrive\onedrive.exe /reset واضغط على موافق.</span><span class="sxs-lookup"><span data-stu-id="3827c-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="3827c-117">قد تظهر نافذة الأمر لفترة قصيرة.</span><span class="sxs-lookup"><span data-stu-id="3827c-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="3827c-118">تشغيل OneDrive يدويا عن طريق الذهاب إلى البدء</span><span class="sxs-lookup"><span data-stu-id="3827c-118">Manually launch OneDrive by going to Start</span></span> ![اضغط على مفتاح Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="3827c-120">، اكتب OneDrive في مربع البحث، ثم انقر فوق تطبيق OneDrive لسطح المكتب.</span><span class="sxs-lookup"><span data-stu-id="3827c-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="3827c-121">ملاحظات:</span><span class="sxs-lookup"><span data-stu-id="3827c-121">Notes:</span></span>

- <span data-ttu-id="3827c-122">إذا اخترت مزامنة بعض المجلدات فقط قبل إعادة التعيين، ستحتاج إلى القيام بذلك مرة أخرى بعد اكتمال المزامنة.</span><span class="sxs-lookup"><span data-stu-id="3827c-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="3827c-123">اقرأ [اختر مجلدات OneDrive التي تريد مزامنتها مع الكمبيوتر للحصول](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)على مزيد من   المعلومات.</span><span class="sxs-lookup"><span data-stu-id="3827c-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="3827c-124">ستحتاج إلى إكمال ذلك ل OneDrive الشخصي و OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="3827c-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>