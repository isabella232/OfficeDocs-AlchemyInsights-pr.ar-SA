---
title: اختناق ترحيل SharePoint باستخدام 503 أخطاء
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931645"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a><span data-ttu-id="71225-102">اختناق ترحيل SharePoint باستخدام 503 أخطاء</span><span class="sxs-lookup"><span data-stu-id="71225-102">SharePoint migration throttling with 503 errors</span></span>

<span data-ttu-id="71225-103">**هام:** يعمل العديد من عملاء SharePoint Online و OneDrive على تشغيل تطبيقات مهمة للأعمال مقابل الخدمة التي تعمل في الخلفية.</span><span class="sxs-lookup"><span data-stu-id="71225-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="71225-104">وتشمل هذه ترحيل المحتوى، منع فقدان البيانات (DLP)، وحلول النسخ الاحتياطي.</span><span class="sxs-lookup"><span data-stu-id="71225-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="71225-105">خلال هذه الأوقات غير المسبوقة، نتخذ خطوات لضمان أن تظل خدمات SharePoint Online و OneDrive متاحة للغاية وموثوقة للمستخدمين الذين يعتمدون على الخدمة أكثر من أي وقت مضى في سيناريوهات العمل عن بعد.</span><span class="sxs-lookup"><span data-stu-id="71225-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="71225-106">ولدعم هذا الهدف، قمنا بتنفيذ قيود خنق أكثر صرامة على تطبيقات الخلفية (الترحيل وDLP وحلول النسخ الاحتياطي) خلال ساعات النهار في أيام الأسبوع.</span><span class="sxs-lookup"><span data-stu-id="71225-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="71225-107">يجب أن تتوقع أن تحقق هذه التطبيقات إنتاجية محدودة جدًا خلال هذه الأوقات.</span><span class="sxs-lookup"><span data-stu-id="71225-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="71225-108">ومع ذلك ، خلال ساعات المساء وعطلة نهاية الأسبوع للمنطقة ، ستكون الخدمة جاهزة لمعالجة حجم أكبر بكثير من الطلبات من تطبيقات الخلفية.</span><span class="sxs-lookup"><span data-stu-id="71225-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="71225-109">**503 أخطاء عند الترحيل إلى SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="71225-109">**503 errors when migrating to SharePoint Online**</span></span>

<span data-ttu-id="71225-110">يبدو أنك تقوم بالترحيل إلى SharePoint Online وتتلقى 503 أخطاء.</span><span class="sxs-lookup"><span data-stu-id="71225-110">It appears you are migrating to SharePoint Online and receiving 503 errors.</span></span> <span data-ttu-id="71225-111">يرجى اتباع الخطوات التالية حتى نتمكن من مساعدتك في أقرب وقت ممكن.</span><span class="sxs-lookup"><span data-stu-id="71225-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="71225-112">انقر فوق **دعم جهة الاتصال،** ثم **طلب خدمة جديد**.</span><span class="sxs-lookup"><span data-stu-id="71225-112">Click **Contact Support**, and then **New Service Request**.</span></span>
2. <span data-ttu-id="71225-113">للعنوان والوصف، اكتب **اختناق ترحيل SharePoint مع 503**.</span><span class="sxs-lookup"><span data-stu-id="71225-113">For the title and description, type **SharePoint Migration Throttling with 503**.</span></span>
3. <span data-ttu-id="71225-114">بمجرد تقديم التذكرة، يرجى تحديثها بالمعلومات التالية:</span><span class="sxs-lookup"><span data-stu-id="71225-114">Once the ticket has been submitted, please update it with the following information:</span></span>
    - <span data-ttu-id="71225-115">كم تبقى من الهجرة (على سبيل المثال، كم TBs؟).</span><span class="sxs-lookup"><span data-stu-id="71225-115">How much left of migration (for example, how many TBs?).</span></span>
    - <span data-ttu-id="71225-116">تاريخ بدء الترحيل ونهايته.</span><span class="sxs-lookup"><span data-stu-id="71225-116">Migration start and end date.</span></span>
    - <span data-ttu-id="71225-117">صف المكان الذي تقوم بترحيل المحتوى الخاص بك منه، مثل SharePoint Server وBox وGDrive ومشاركات الملفات وما إلى ذلك.</span><span class="sxs-lookup"><span data-stu-id="71225-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>
    - <span data-ttu-id="71225-118">تقدير عدد أخطاء الاختناق (على سبيل المثال، س خنق في الساعة؟) ومتى حدث الاختناق.</span><span class="sxs-lookup"><span data-stu-id="71225-118">Estimate the number of throttling errors (for example, x throttle per hour?) and when did the throttling happen.</span></span>
    - <span data-ttu-id="71225-119">أداة الترحيل التي تستخدمها (على سبيل المثال، SPMT أو ShareGate).</span><span class="sxs-lookup"><span data-stu-id="71225-119">Which migration tool you are using (for example, SPMT or ShareGate).</span></span>


