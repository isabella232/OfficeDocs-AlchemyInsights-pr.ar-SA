---
title: Microsoft Edge تكوين إعدادات الخصوصية
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/08/2020
ms.locfileid: "49676709"
---
# <a name="microsoft-edge-configure-privacy-settings"></a><span data-ttu-id="1e0a5-102">Microsoft Edge تكوين إعدادات الخصوصية</span><span class="sxs-lookup"><span data-stu-id="1e0a5-102">Microsoft Edge configure privacy settings</span></span>

<span data-ttu-id="1e0a5-103">بشكل افتراضي ، إذا تم نشر Microsoft Edge علي الانظمه الاساسيه غير التابعة لنظام التشغيل Windows ، فلن يتم إرسال البيانات التشخيصية ومعلومات الموقع إلى Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1e0a5-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information are not sent to Microsoft.</span></span> <span data-ttu-id="1e0a5-104">ومع ذلك ، إذا تم نشر Microsoft Edge علي Windows 10 ، سيتم إرسال بيانات التشخيص ومعلومات الموقع وفقا [لإعدادات بيانات تشخيص Windows](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)الخاصة بالمستخدمين.</span><span class="sxs-lookup"><span data-stu-id="1e0a5-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span></span>

<span data-ttu-id="1e0a5-105">لتكوين الطريقة التي يتعامل بها Microsoft Edge مع مجموعه البيانات لمؤسسك ، استخدم نهج المجموعة التالية:</span><span class="sxs-lookup"><span data-stu-id="1e0a5-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="1e0a5-106">[ميتريكسريبورتينجينابليد](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): يؤدي هذا النهج إلى تمكين اعداد تقارير الاستخدام والبيانات ذات الصلة بالعطل.</span><span class="sxs-lookup"><span data-stu-id="1e0a5-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): This policy enables reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="1e0a5-107">[سيندسيتينفوتويمبروفيسيرفيسيس](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): يقوم هذا النهج بإرسال معلومات الموقع المستخدمة لتحسين خدمات Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1e0a5-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): This policy sends site information that is used to improve Microsoft services.</span></span>

<span data-ttu-id="1e0a5-108">لمعرفه المزيد ، راجع [تكوين إعدادات النهج](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span><span class="sxs-lookup"><span data-stu-id="1e0a5-108">To learn more, see [Configure policy settings](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span></span>