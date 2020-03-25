---
title: ترحيل الخيارات إلى SharePoint Online
ms.author: pebaum
author: v-miegge
manager: v-cojank
ms.date: 11/04/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: c8c339c9-2e50-4daa-aa91-3eb5053e2bc6
ms.openlocfilehash: 830b39c51658cbc02f4be81acdfdf3b164a8df70
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932717"
---
# <a name="migrate-options-to-sharepoint-online"></a><span data-ttu-id="48f5a-102">ترحيل الخيارات إلى SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="48f5a-102">Migrate options to SharePoint Online</span></span>

<span data-ttu-id="48f5a-103">**هام:** يعمل العديد من عملاء SharePoint Online و OneDrive على تشغيل تطبيقات مهمة للأعمال مقابل الخدمة التي تعمل في الخلفية.</span><span class="sxs-lookup"><span data-stu-id="48f5a-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="48f5a-104">وتشمل هذه ترحيل المحتوى، منع فقدان البيانات (DLP)، وحلول النسخ الاحتياطي.</span><span class="sxs-lookup"><span data-stu-id="48f5a-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="48f5a-105">خلال هذه الأوقات غير المسبوقة، نتخذ خطوات لضمان أن تظل خدمات SharePoint Online و OneDrive متاحة للغاية وموثوقة للمستخدمين الذين يعتمدون على الخدمة أكثر من أي وقت مضى في سيناريوهات العمل عن بعد.</span><span class="sxs-lookup"><span data-stu-id="48f5a-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="48f5a-106">ولدعم هذا الهدف، قمنا بتنفيذ قيود خنق أكثر صرامة على تطبيقات الخلفية (الترحيل وDLP وحلول النسخ الاحتياطي) خلال ساعات النهار في أيام الأسبوع.</span><span class="sxs-lookup"><span data-stu-id="48f5a-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="48f5a-107">يجب أن تتوقع أن تحقق هذه التطبيقات إنتاجية محدودة جدًا خلال هذه الأوقات.</span><span class="sxs-lookup"><span data-stu-id="48f5a-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="48f5a-108">ومع ذلك ، خلال ساعات المساء وعطلة نهاية الأسبوع للمنطقة ، ستكون الخدمة جاهزة لمعالجة حجم أكبر بكثير من الطلبات من تطبيقات الخلفية.</span><span class="sxs-lookup"><span data-stu-id="48f5a-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="48f5a-109">**خيارات الترحيل**</span><span class="sxs-lookup"><span data-stu-id="48f5a-109">**Migration options**</span></span>

<span data-ttu-id="48f5a-110">هناك خيارات مختلفة متاحة لترحيل المحتوى إلى SharePoint Online ، اعتمادًا على حجم وكمية الملفات التي تحتاج إلى نقلها ، يرجى الاطلاع على قائمة بالخيارات [الموجودة هنا](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="48f5a-110">There are different options available to migrate content to SharePoint Online, depending on the size and quantity of files you need to move, please see a list of options [located here](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span></span>

<span data-ttu-id="48f5a-111">لمزيد من المعلومات حول ترحيل المحتوى، يرجى زيارة الروابط أدناه.</span><span class="sxs-lookup"><span data-stu-id="48f5a-111">For more information on content migration, please visit the links below.</span></span>

- [<span data-ttu-id="48f5a-112">أداة ترحيل نقطة المشاركة</span><span class="sxs-lookup"><span data-stu-id="48f5a-112">Sharepoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)

- [<span data-ttu-id="48f5a-113">ابدأ مع مدير الترحيل</span><span class="sxs-lookup"><span data-stu-id="48f5a-113">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="48f5a-114">Sharepoint عبر الإنترنت وسرعة الهجرة ODB</span><span class="sxs-lookup"><span data-stu-id="48f5a-114">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="48f5a-115">تجنب الحصول على خنق أو حظر في SharePoint عبر الإنترنت</span><span class="sxs-lookup"><span data-stu-id="48f5a-115">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="48f5a-116">أداة تقييم ترحيل SharePoint (SMAT)</span><span class="sxs-lookup"><span data-stu-id="48f5a-116">SharePoint Migration Assessment Tool (SMAT)</span></span>](https://www.microsoft.com/download/details.aspx?id=53598&amp;751be11f-ede8-5a0c-058c-2ee190a24fa6=True)

<span data-ttu-id="48f5a-117">**ملاحظة:** حالياً تدعم أداة ترحيل SharePoint عمليات الترحيل من SharePoint 2010 و 2013 فقط.</span><span class="sxs-lookup"><span data-stu-id="48f5a-117">**Note**: Currently the SharePoint Migration tool only support migrations from SharePoint 2010  and 2013.</span></span> <span data-ttu-id="48f5a-118">الإصدار 2016 أو 2019 غير معتمد في الوقت الحالي.</span><span class="sxs-lookup"><span data-stu-id="48f5a-118">Version 2016 or 2019 are not supported at this time.</span></span>
