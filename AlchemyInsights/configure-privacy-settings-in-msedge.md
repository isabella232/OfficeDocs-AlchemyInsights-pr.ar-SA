---
title: تكوين إعدادات الخصوصية في Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404192"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a><span data-ttu-id="92881-102">تكوين إعدادات الخصوصية في Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="92881-102">Configure privacy settings in Microsoft Edge</span></span>

<span data-ttu-id="92881-103">بشكل افتراضي، إذا تم نشر Microsoft Edge على الأنظمة الأساسية غير التي تعمل بنظام التشغيل Windows، لا يتم إرسال البيانات التشخيصية ومعلومات الموقع إلى Microsoft.</span><span class="sxs-lookup"><span data-stu-id="92881-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information aren't sent to Microsoft.</span></span> <span data-ttu-id="92881-104">ومع ذلك، إذا تم نشر Microsoft Edge على Windows 10، يتم إرسال البيانات التشخيصية ومعلومات الموقع وفقا لإعدادات بيانات [Windows التشخيصية للمستخدمين.](https://go.microsoft.com/fwlink/?linkid=2132472)</span><span class="sxs-lookup"><span data-stu-id="92881-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://go.microsoft.com/fwlink/?linkid=2132472).</span></span>

<span data-ttu-id="92881-105">لتكوين كيفية معالجة Microsoft Edge لجمع البيانات لمجموعتك، استخدم سياسات المجموعة التالية:</span><span class="sxs-lookup"><span data-stu-id="92881-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="92881-106">[المقاييسReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) تشغيل الإبلاغ عن الاستخدام والبيانات ذات الصلة بالتعطل.</span><span class="sxs-lookup"><span data-stu-id="92881-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) turns on reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="92881-107">[ترسل SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) معلومات الموقع المستخدمة لتحسين خدمات Microsoft.</span><span class="sxs-lookup"><span data-stu-id="92881-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) sends site information used to improve Microsoft services.</span></span>

<span data-ttu-id="92881-108">لمعرفة المزيد، راجع [تكوين إعدادات النهج](https://go.microsoft.com/fwlink/?linkid=2132577).</span><span class="sxs-lookup"><span data-stu-id="92881-108">To learn more, see [Configure policy settings](https://go.microsoft.com/fwlink/?linkid=2132577).</span></span>
