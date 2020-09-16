---
title: استكشاف أخطاء تعطل OneDrive وإصلاحها
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664985"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="59c1e-102">استكشاف أخطاء تعطل OneDrive وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="59c1e-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="59c1e-103">إذا تعطل OneDrive بشكل متكرر ، فجرب خطوات استكشاف الأخطاء وإصلاحها هذه:</span><span class="sxs-lookup"><span data-stu-id="59c1e-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="59c1e-104">**تاكد من عدم تعيين مفاتيح التسجيل:**</span><span class="sxs-lookup"><span data-stu-id="59c1e-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="59c1e-105">باستخدام "محرر السجل" ، انتقل إلى HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="59c1e-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="59c1e-106">إذا كانت ديسابليفيليسينكنجسك موجودة وتم تعيينها إلى 1 ، فافتح المفتاح وغير القيمة إلى 0.</span><span class="sxs-lookup"><span data-stu-id="59c1e-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="59c1e-107">تشغيل OneDrive يدويا بالانتقال إلى البدء</span><span class="sxs-lookup"><span data-stu-id="59c1e-107">Manually launch OneDrive by going to Start</span></span> ![اضغط علي مفتاح Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="59c1e-109">، واكتب OneDrive في مربع البحث ، ثم انقر فوق تطبيق OneDrive لسطح المكتب.</span><span class="sxs-lookup"><span data-stu-id="59c1e-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="59c1e-110">**أعاده تعيين OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="59c1e-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="59c1e-111">"</span><span class="sxs-lookup"><span data-stu-id="59c1e-111">Notes:</span></span>

- <span data-ttu-id="59c1e-112">تؤدي أعاده تعيين OneDrive إلى قطع جميع اتصالات المزامنة الحالية (بما في ذلك OneDrive الشخصي في حاله اعداده).</span><span class="sxs-lookup"><span data-stu-id="59c1e-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="59c1e-113">لن تفقد الملفات أو البيانات عن طريق أعاده تعيين OneDrive علي الكمبيوتر.</span><span class="sxs-lookup"><span data-stu-id="59c1e-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="59c1e-114">**لأعاده تعيين OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="59c1e-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="59c1e-115">افتح مربع الحوار "تشغيل" بالضغط علي مفتاح Windows و R.</span><span class="sxs-lookup"><span data-stu-id="59c1e-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="59c1e-116">اكتب% لوكالابداتا% \Microsoft\OneDrive\onedrive.exe/أعاده تعيين واضغط علي موافق.</span><span class="sxs-lookup"><span data-stu-id="59c1e-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="59c1e-117">قد تظهر نافذه الأوامر باختصار.</span><span class="sxs-lookup"><span data-stu-id="59c1e-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="59c1e-118">تشغيل OneDrive يدويا بالانتقال إلى البدء</span><span class="sxs-lookup"><span data-stu-id="59c1e-118">Manually launch OneDrive by going to Start</span></span> ![اضغط علي مفتاح Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="59c1e-120">، واكتب OneDrive في مربع البحث ، ثم انقر فوق تطبيق OneDrive لسطح المكتب.</span><span class="sxs-lookup"><span data-stu-id="59c1e-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="59c1e-121">"</span><span class="sxs-lookup"><span data-stu-id="59c1e-121">Notes:</span></span>

- <span data-ttu-id="59c1e-122">إذا اخترت مزامنة بعض المجلدات فقط قبل أعاده التعيين ، ستحتاج إلى القيام بذلك مره أخرى بعد اكتمال المزامنة.</span><span class="sxs-lookup"><span data-stu-id="59c1e-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="59c1e-123">أقرا [اختيار مجلدات OneDrive المراد مزامنتها مع الكمبيوتر](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   للحصول علي مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="59c1e-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="59c1e-124">ستحتاج إلى إكمال هذا الاجراء ل OneDrive و OneDrive for Business الشخصي.</span><span class="sxs-lookup"><span data-stu-id="59c1e-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>