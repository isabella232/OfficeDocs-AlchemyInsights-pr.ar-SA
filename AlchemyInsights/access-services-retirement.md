---
title: التقاعد في Access services
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698633"
---
# <a name="access-services-retirement"></a><span data-ttu-id="ca91e-102">التقاعد في Access services</span><span class="sxs-lookup"><span data-stu-id="ca91e-102">Access services retirement</span></span>

<span data-ttu-id="ca91e-103">بما اننا إعلاننا بالفعل في MC97576 ، وفي مارس 2017 ، ومستمر للتواصل عبر السنه الماضية ، سيتم إيقاف خدمه Access.</span><span class="sxs-lookup"><span data-stu-id="ca91e-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="ca91e-104">ستكون المرحلة التالية في هذه العملية هي أزاله قواعد بيانات Access علي ويب التي تستخدم قوائم SharePoint كمساحة تخزين البيانات الاساسيه الخاصة بها.</span><span class="sxs-lookup"><span data-stu-id="ca91e-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="ca91e-105">**كيف يؤثر هذا ؟**</span><span class="sxs-lookup"><span data-stu-id="ca91e-105">**How does this affect me?**</span></span>

<span data-ttu-id="ca91e-106">بدءا من يونيو 2019 ، سنقوم بإيقاف إنشاء قواعد بيانات Access جديده في SharePoint Online وإيقاف تشغيل الخدمة وأي تطبيقات متبقية بحلول ابريل 2020.</span><span class="sxs-lookup"><span data-stu-id="ca91e-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="ca91e-107">**ما الذي احتاج إلى فعله للتحضير لهذا التغيير ؟**</span><span class="sxs-lookup"><span data-stu-id="ca91e-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="ca91e-108">نحن نشجعك علي إنشاء خطه انتقال لقواعد بيانات Access علي ويب الخاصة بمؤسسك.</span><span class="sxs-lookup"><span data-stu-id="ca91e-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="ca91e-109">يمكن للمسؤولين استخدام [ماسح تطبيق SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) للحصول علي مخزون تطبيقات Access التي تستخدمها المواقع.</span><span class="sxs-lookup"><span data-stu-id="ca91e-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="ca91e-110">هناك طرق متعددة لترحيل بيانات قواعد بيانات Access علي الويب:</span><span class="sxs-lookup"><span data-stu-id="ca91e-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="ca91e-111">الاستيراد إلى قاعده بيانات Access محليه (. ACCDB) أو إلى ملف Excel.</span><span class="sxs-lookup"><span data-stu-id="ca91e-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="ca91e-112">نوصي أيضا باستكشاف Microsoft PowerApps كنظام أساسي بديل لإنشاء حلول للشركات التي لا تستخدم التعليمات البرمجية للاجهزه المحمولة والويب.</span><span class="sxs-lookup"><span data-stu-id="ca91e-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>