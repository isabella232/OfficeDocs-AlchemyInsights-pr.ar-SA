---
title: الحصول على خدمات التقاعد
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 197366882468ebc87fc26f2fe2733371790d1871
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36747771"
---
# <a name="access-services-retirement"></a><span data-ttu-id="45bae-102">الحصول على خدمات التقاعد</span><span class="sxs-lookup"><span data-stu-id="45bae-102">Access services retirement</span></span>

<span data-ttu-id="45bae-103">كما أعلنا في الأصل في MC97576، في مارس 2017، واستمر في التواصل على مدى العام الماضي يتم سحب خدمات الوصول من Office 365.</span><span class="sxs-lookup"><span data-stu-id="45bae-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="45bae-104">ستكون المرحلة التالية في هذه العملية إزالة قواعد بيانات ويب Access التي تستخدم قوائم SharePoint كتخزين البيانات الأساسية الخاصة بهم.</span><span class="sxs-lookup"><span data-stu-id="45bae-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="45bae-105">**كيف يؤثر هذا علي؟**</span><span class="sxs-lookup"><span data-stu-id="45bae-105">**How does this affect me?**</span></span>

<span data-ttu-id="45bae-106">بدءًا من يونيو 2019، سنقوم بإيقاف إنشاء قواعد بيانات Access جديدة في SharePoint Online وإيقاف تشغيل الخدمة وأي تطبيقات متبقية بحلول أبريل 2020.</span><span class="sxs-lookup"><span data-stu-id="45bae-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="45bae-107">**ماذا يجب أن أفعل للاستعداد لهذا التغيير؟**</span><span class="sxs-lookup"><span data-stu-id="45bae-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="45bae-108">ونحن نشجعك على إنشاء خطة انتقال لقواعد بيانات ويب Access الخاصة بمؤسستك.</span><span class="sxs-lookup"><span data-stu-id="45bae-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="45bae-109">يمكن للمسؤولين استخدام [الماسح الضوئي التطبيق SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) للحصول على مخزون من تطبيقات Access التي تستخدمها المواقع.</span><span class="sxs-lookup"><span data-stu-id="45bae-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="45bae-110">هناك عدة طرق لترحيل بيانات قواعد بيانات ويب Access:</span><span class="sxs-lookup"><span data-stu-id="45bae-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="45bae-111">الاستيراد إلى قاعدة بيانات Access محلية (. ACCDB) أو إلى ملف Excel.</span><span class="sxs-lookup"><span data-stu-id="45bae-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="45bae-112">نوصي أيضًا باستكشاف Microsoft PowerApps كمنصة بديلة لإنشاء حلول أعمال بدون رموز للأجهزة الويب والمحمولة.</span><span class="sxs-lookup"><span data-stu-id="45bae-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>