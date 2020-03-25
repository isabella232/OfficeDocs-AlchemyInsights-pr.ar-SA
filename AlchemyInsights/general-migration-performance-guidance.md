---
title: إرشادات عامة حول أداء الترحيل
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3179"
ms.openlocfilehash: 10a0069c41d2e5128b2592425d815364a83b730f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932466"
---
# <a name="general-migration-performance-guidance"></a><span data-ttu-id="03169-102">إرشادات عامة حول أداء الترحيل</span><span class="sxs-lookup"><span data-stu-id="03169-102">General migration performance guidance</span></span>

<span data-ttu-id="03169-103">**هام**: يقوم العديد من عملاء SharePoint Online وOneDrive بتشغيل تطبيقات هامة للأعمال بالتوازي مع الخدمات التي يتم تشغيلها في الخلفية.</span><span class="sxs-lookup"><span data-stu-id="03169-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="03169-104">حيث تتضمن ترحيل المحتوى وتفادي فقدان البيانات (DLP) وحلول النسخ الاحتياطي.</span><span class="sxs-lookup"><span data-stu-id="03169-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="03169-105">خلال هذه الأوقات غير المسبوقة، سنقوم باتخاذ الخطوات التالية لضمان بقاء خدمات SharePoint Online و OneDrive متوفرة على مستوى عالٍ من الجودة والوثوقية للمستخدمين الذين يعتمدون على تلك الخدمات أكثر من ذي قبل في سيناريوهات العمل عن بُعد.</span><span class="sxs-lookup"><span data-stu-id="03169-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="03169-106">لدعم هذا الهدف، قمنا بتطبيق تقييد أكبر على التطبيقات الخلفية (الترحيل وتفادي فقدان البيانات (DLP) وحلول النسخ الاحتياطي) خلال ساعات النهار من أيام العمل.</span><span class="sxs-lookup"><span data-stu-id="03169-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="03169-107">يجب أن تضع في حسبانك أن هذه التطبيقات سيكون معدل نقلها محدوداً جداً خلال هذه الأوقات.</span><span class="sxs-lookup"><span data-stu-id="03169-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="03169-108">وعلى الرغم من ذلك، ستكون الخدمة جاهزة لمعالجة حجم أكبر من طلبات التطبيقات الخلفية أثناء المساء وساعات نهاية الأسبوع في منطقتك.</span><span class="sxs-lookup"><span data-stu-id="03169-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="03169-109">**إرشادات حول أداء الترحيل**</span><span class="sxs-lookup"><span data-stu-id="03169-109">**Migration performance guidance**</span></span>

<span data-ttu-id="03169-110">يمكن أن يتأثر أداء الترحيل بالبنية الأساسية للشبكة وحجم الملف ووقت الترحيل والتقييد.</span><span class="sxs-lookup"><span data-stu-id="03169-110">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling.</span></span> <span data-ttu-id="03169-111">سيساعدك معرفة ذلك في تخطيط الترحيل وزيادة فعاليته.</span><span class="sxs-lookup"><span data-stu-id="03169-111">Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

- [<span data-ttu-id="03169-112">إرشادات عامة حول أداء الترحيل</span><span class="sxs-lookup"><span data-stu-id="03169-112">General migration performance guidance</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)
