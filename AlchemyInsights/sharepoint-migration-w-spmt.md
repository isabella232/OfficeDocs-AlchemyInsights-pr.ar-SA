---
title: ترحيل SharePoint باستخدام SPMT
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2594"
ms.openlocfilehash: e7719d1fc6dda0d5bd340775219401dade2933fe
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931537"
---
# <a name="sharepoint-migration-with-spmt"></a><span data-ttu-id="4ba1a-102">ترحيل SharePoint باستخدام SPMT</span><span class="sxs-lookup"><span data-stu-id="4ba1a-102">SharePoint Migration with SPMT</span></span>

<span data-ttu-id="4ba1a-103">**هام:** يعمل العديد من عملاء SharePoint Online و OneDrive على تشغيل تطبيقات مهمة للأعمال مقابل الخدمة التي تعمل في الخلفية.</span><span class="sxs-lookup"><span data-stu-id="4ba1a-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="4ba1a-104">وتشمل هذه ترحيل المحتوى، منع فقدان البيانات (DLP)، وحلول النسخ الاحتياطي.</span><span class="sxs-lookup"><span data-stu-id="4ba1a-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="4ba1a-105">خلال هذه الأوقات غير المسبوقة، نتخذ خطوات لضمان أن تظل خدمات SharePoint Online و OneDrive متاحة للغاية وموثوقة للمستخدمين الذين يعتمدون على الخدمة أكثر من أي وقت مضى في سيناريوهات العمل عن بعد.</span><span class="sxs-lookup"><span data-stu-id="4ba1a-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="4ba1a-106">ولدعم هذا الهدف، قمنا بتنفيذ قيود خنق أكثر صرامة على تطبيقات الخلفية (الترحيل وDLP وحلول النسخ الاحتياطي) خلال ساعات النهار في أيام الأسبوع.</span><span class="sxs-lookup"><span data-stu-id="4ba1a-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="4ba1a-107">يجب أن تتوقع أن تحقق هذه التطبيقات إنتاجية محدودة جدًا خلال هذه الأوقات.</span><span class="sxs-lookup"><span data-stu-id="4ba1a-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="4ba1a-108">ومع ذلك ، خلال ساعات المساء وعطلة نهاية الأسبوع للمنطقة ، ستكون الخدمة جاهزة لمعالجة حجم أكبر بكثير من الطلبات من تطبيقات الخلفية.</span><span class="sxs-lookup"><span data-stu-id="4ba1a-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="4ba1a-109">**أداة ترحيل SharePoint**</span><span class="sxs-lookup"><span data-stu-id="4ba1a-109">**SharePoint Migration Tool**</span></span>

<span data-ttu-id="4ba1a-110">مصممة لاستخدامها في عمليات الترحيل التي تتراوح بين أصغر مجموعة من الملفات إلى ترحيل المؤسسة على نطاق واسع، ستسمح لك أداة ترحيل SharePoint بنقل معلوماتك إلى السحابة والاستفادة من أحدث تعاون وذكاء و حلول الأمان مع Office 365.</span><span class="sxs-lookup"><span data-stu-id="4ba1a-110">Designed to be used for migrations ranging from the smallest set of files to a large scale enterprise migration, the SharePoint Migration Tool will allow you to transfer your information to the cloud and take advantage of the newest collaboration, intelligence, and security solutions with Office 365.</span></span>

- [<span data-ttu-id="4ba1a-111">تنزيل أداة ترحيل SharePoint وتثبيتها</span><span class="sxs-lookup"><span data-stu-id="4ba1a-111">Download and install the SharePoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
- [<span data-ttu-id="4ba1a-112">استكشاف مشكلات SPMT الشائعة وإصلاحها والأخطاء</span><span class="sxs-lookup"><span data-stu-id="4ba1a-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
- [<span data-ttu-id="4ba1a-113">استكشاف مشكلات تثبيت SPMT وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="4ba1a-113">Troubleshooting SPMT installation issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues#troubleshooting-spmt-installation-issues)
