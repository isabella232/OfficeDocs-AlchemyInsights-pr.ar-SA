---
title: SharePoint على الانترنت اختناق
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 9af4f09d50992c04a1f3d5a164093049a3ec3517
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931429"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="1f0bd-102">SharePoint على الانترنت اختناق</span><span class="sxs-lookup"><span data-stu-id="1f0bd-102">SharePoint Online throttling</span></span>

<span data-ttu-id="1f0bd-103">**هام:** يعمل العديد من عملاء SharePoint Online و OneDrive على تشغيل تطبيقات مهمة للأعمال مقابل الخدمة التي تعمل في الخلفية.</span><span class="sxs-lookup"><span data-stu-id="1f0bd-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="1f0bd-104">وتشمل هذه ترحيل المحتوى، منع فقدان البيانات (DLP)، وحلول النسخ الاحتياطي.</span><span class="sxs-lookup"><span data-stu-id="1f0bd-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="1f0bd-105">خلال هذه الأوقات غير المسبوقة، نتخذ خطوات لضمان أن تظل خدمات SharePoint Online و OneDrive متاحة للغاية وموثوقة للمستخدمين الذين يعتمدون على الخدمة أكثر من أي وقت مضى في سيناريوهات العمل عن بعد.</span><span class="sxs-lookup"><span data-stu-id="1f0bd-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="1f0bd-106">ولدعم هذا الهدف، قمنا بتنفيذ قيود خنق أكثر صرامة على تطبيقات الخلفية (الترحيل وDLP وحلول النسخ الاحتياطي) خلال ساعات النهار في أيام الأسبوع.</span><span class="sxs-lookup"><span data-stu-id="1f0bd-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="1f0bd-107">يجب أن تتوقع أن تحقق هذه التطبيقات إنتاجية محدودة جدًا خلال هذه الأوقات.</span><span class="sxs-lookup"><span data-stu-id="1f0bd-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="1f0bd-108">ومع ذلك ، خلال ساعات المساء وعطلة نهاية الأسبوع للمنطقة ، ستكون الخدمة جاهزة لمعالجة حجم أكبر بكثير من الطلبات من تطبيقات الخلفية.</span><span class="sxs-lookup"><span data-stu-id="1f0bd-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="1f0bd-109">**SharePoint على الانترنت اختناق**</span><span class="sxs-lookup"><span data-stu-id="1f0bd-109">**SharePoint Online throttling**</span></span>

<span data-ttu-id="1f0bd-110">يستخدم SharePoint Online الاختناق للحفاظ على الأداء الأمثل وموثوقية خدمة SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="1f0bd-110">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="1f0bd-111">الاختناق يحد من عدد إجراءات المستخدم أو المكالمات المتزامنة (بواسطة البرنامج النصي أو التعليمات البرمجية) لمنع الإفراط في استخدام الموارد.</span><span class="sxs-lookup"><span data-stu-id="1f0bd-111">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="1f0bd-112">لمزيد من المعلومات، يرجى زيارة الروابط أدناه.</span><span class="sxs-lookup"><span data-stu-id="1f0bd-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="1f0bd-113">تجنب الحصول على خنق أو حظر في SharePoint عبر الإنترنت</span><span class="sxs-lookup"><span data-stu-id="1f0bd-113">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="1f0bd-114">ترحيل البيانات واختناق SPO</span><span class="sxs-lookup"><span data-stu-id="1f0bd-114">Data Migration and SPO Throttling </span></span>](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)

- [<span data-ttu-id="1f0bd-115">SharePoint عبر الإنترنت وOneDrive سرعة الترحيل</span><span class="sxs-lookup"><span data-stu-id="1f0bd-115">SharePoint Online and OneDrive Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

 - [<span data-ttu-id="1f0bd-116">التعامل مع اختناق SharePoint Online باستخدام التراجع الأسي</span><span class="sxs-lookup"><span data-stu-id="1f0bd-116">Handle SharePoint Online throttling by using exponential back off</span></span>](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)

- [<span data-ttu-id="1f0bd-117">تخطيط القدرات واختبار التحميل SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="1f0bd-117">Capacity planning and load testing SharePoint Online</span></span>](https://docs.microsoft.com/office365/enterprise/capacity-planning-and-load-testing-sharepoint-online)

