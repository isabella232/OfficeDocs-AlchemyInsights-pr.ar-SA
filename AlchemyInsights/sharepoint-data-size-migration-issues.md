---
title: مشكلات أثناء ترحيل البيانات إلى SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "1885"
ms.openlocfilehash: b53a98480bab48497274c7358f7e606caa477f5a
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931681"
---
# <a name="issues-while-migrating-data-to-sharepoint-online"></a><span data-ttu-id="f30a0-102">مشكلات أثناء ترحيل البيانات إلى SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="f30a0-102">Issues while migrating data to SharePoint Online</span></span>

<span data-ttu-id="f30a0-103">**هام:** يعمل العديد من عملاء SharePoint Online و OneDrive على تشغيل تطبيقات مهمة للأعمال مقابل الخدمة التي تعمل في الخلفية.</span><span class="sxs-lookup"><span data-stu-id="f30a0-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="f30a0-104">وتشمل هذه ترحيل المحتوى، منع فقدان البيانات (DLP)، وحلول النسخ الاحتياطي.</span><span class="sxs-lookup"><span data-stu-id="f30a0-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="f30a0-105">خلال هذه الأوقات غير المسبوقة، نتخذ خطوات لضمان أن تظل خدمات SharePoint Online و OneDrive متاحة للغاية وموثوقة للمستخدمين الذين يعتمدون على الخدمة أكثر من أي وقت مضى في سيناريوهات العمل عن بعد.</span><span class="sxs-lookup"><span data-stu-id="f30a0-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="f30a0-106">ولدعم هذا الهدف، قمنا بتنفيذ قيود خنق أكثر صرامة على تطبيقات الخلفية (الترحيل وDLP وحلول النسخ الاحتياطي) خلال ساعات النهار في أيام الأسبوع.</span><span class="sxs-lookup"><span data-stu-id="f30a0-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="f30a0-107">يجب أن تتوقع أن تحقق هذه التطبيقات إنتاجية محدودة جدًا خلال هذه الأوقات.</span><span class="sxs-lookup"><span data-stu-id="f30a0-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="f30a0-108">ومع ذلك ، خلال ساعات المساء وعطلة نهاية الأسبوع للمنطقة ، ستكون الخدمة جاهزة لمعالجة حجم أكبر بكثير من الطلبات من تطبيقات الخلفية.</span><span class="sxs-lookup"><span data-stu-id="f30a0-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="f30a0-109">**ترحيل أكثر من 100 تيرابايت من البيانات**</span><span class="sxs-lookup"><span data-stu-id="f30a0-109">**Migrating over 100TB of data**</span></span>

<span data-ttu-id="f30a0-110">يبدو أنك تقوم بترحيل أكثر من 100 تيرابايت من البيانات إلى SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="f30a0-110">It appears you are migrating over 100TB of data to SharePoint Online.</span></span> <span data-ttu-id="f30a0-111">يرجى اتباع الخطوات التالية حتى نتمكن من مساعدتك في أقرب وقت ممكن.</span><span class="sxs-lookup"><span data-stu-id="f30a0-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="f30a0-112">حدد **طلب خدمة جديد،** ثم **طلب خدمة جديد**.</span><span class="sxs-lookup"><span data-stu-id="f30a0-112">Select **New Service Request**, and then **New Service Request**.</span></span> 
2. <span data-ttu-id="f30a0-113">اترك العنوان والوصف **كترحيل SharePoint أكثر من 100 تيرابايت**.</span><span class="sxs-lookup"><span data-stu-id="f30a0-113">Leave the title and description as **SharePoint migration over 100TB**.</span></span>
3. <span data-ttu-id="f30a0-114">بمجرد تقديم التذكرة، يرجى تحديثها بالمعلومات التالية:</span><span class="sxs-lookup"><span data-stu-id="f30a0-114">Once the ticket has been submitted, please update it with the following information:</span></span> 

    - <span data-ttu-id="f30a0-115">الحجم المقدر للترحيل.</span><span class="sxs-lookup"><span data-stu-id="f30a0-115">Estimated size of your migration.</span></span>
    - <span data-ttu-id="f30a0-116">تقدير للموعد الذي ترغب في بدء الترحيل وإكماله.</span><span class="sxs-lookup"><span data-stu-id="f30a0-116">An estimate of when you would like to start and complete your migration.</span></span>
    - <span data-ttu-id="f30a0-117">صف المكان الذي تقوم بترحيل المحتوى الخاص بك منه، مثل SharePoint Server وBox وGDrive ومشاركات الملفات وما إلى ذلك.</span><span class="sxs-lookup"><span data-stu-id="f30a0-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>


  

