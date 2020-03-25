---
title: استكشاف مشكلات وأخطاء أداة ترحيل SharePoint وإصلاحها
ms.author: v-miegge
author: v-miegge
manager: v-cojank
ms.date: 10/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3178"
ms.assetid: ''
ms.openlocfilehash: f9f5694b1d88bccebdc5448d5629ea5120c52511
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931105"
---
# <a name="troubleshooting-sharepoint-migration-tool-issues-and-errors"></a><span data-ttu-id="92c27-102">استكشاف مشكلات وأخطاء أداة ترحيل SharePoint وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="92c27-102">Troubleshooting SharePoint Migration Tool issues and errors</span></span>

<span data-ttu-id="92c27-103">**هام:** يعمل العديد من عملاء SharePoint Online و OneDrive على تشغيل تطبيقات مهمة للأعمال مقابل الخدمة التي تعمل في الخلفية.</span><span class="sxs-lookup"><span data-stu-id="92c27-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="92c27-104">وتشمل هذه ترحيل المحتوى، منع فقدان البيانات (DLP)، وحلول النسخ الاحتياطي.</span><span class="sxs-lookup"><span data-stu-id="92c27-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="92c27-105">خلال هذه الأوقات غير المسبوقة، نتخذ خطوات لضمان أن تظل خدمات SharePoint Online و OneDrive متاحة للغاية وموثوقة للمستخدمين الذين يعتمدون على الخدمة أكثر من أي وقت مضى في سيناريوهات العمل عن بعد.</span><span class="sxs-lookup"><span data-stu-id="92c27-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="92c27-106">ولدعم هذا الهدف، قمنا بتنفيذ قيود خنق أكثر صرامة على تطبيقات الخلفية (الترحيل وDLP وحلول النسخ الاحتياطي) خلال ساعات النهار في أيام الأسبوع.</span><span class="sxs-lookup"><span data-stu-id="92c27-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="92c27-107">يجب أن تتوقع أن تحقق هذه التطبيقات إنتاجية محدودة جدًا خلال هذه الأوقات.</span><span class="sxs-lookup"><span data-stu-id="92c27-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="92c27-108">ومع ذلك ، خلال ساعات المساء وعطلة نهاية الأسبوع للمنطقة ، ستكون الخدمة جاهزة لمعالجة حجم أكبر بكثير من الطلبات من تطبيقات الخلفية.</span><span class="sxs-lookup"><span data-stu-id="92c27-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="92c27-109">**المشكلات والأخطاء الشائعة**</span><span class="sxs-lookup"><span data-stu-id="92c27-109">**Common issues and errors**</span></span>

<span data-ttu-id="92c27-110">قد تواجه بعض المشكلات والأخطاء الشائعة عند استخدام أداة ترحيل SharePoint (SPMT).</span><span class="sxs-lookup"><span data-stu-id="92c27-110">You may encounter some common issues and errors when using the SharePoint Migration Tool (SPMT).</span></span> <span data-ttu-id="92c27-111">يرجى الرجوع إلى الروابط أدناه لمزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="92c27-111">Please reference the links below for more information.</span></span>

* [<span data-ttu-id="92c27-112">استكشاف مشكلات SPMT الشائعة وإصلاحها والأخطاء</span><span class="sxs-lookup"><span data-stu-id="92c27-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
* [<span data-ttu-id="92c27-113">استكشاف مشكلات تثبيت SPMT استكشاف الأخطاء وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="92c27-113">Troubleshooting SPMT install issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues)