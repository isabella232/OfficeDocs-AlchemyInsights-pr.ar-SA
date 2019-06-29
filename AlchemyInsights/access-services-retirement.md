---
title: الوصول إلى خدمات التقاعد
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 5f171050479f34077f3dc155bec40437f86b84c0
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/28/2019
ms.locfileid: "35359321"
---
# <a name="access-services-retirement"></a><span data-ttu-id="3e36a-102">الوصول إلى خدمات التقاعد</span><span class="sxs-lookup"><span data-stu-id="3e36a-102">Access services retirement</span></span>

<span data-ttu-id="3e36a-103">ونحن أصلاً في MC97576، وأعلن في آذار/مارس عام 2017، وتواصل الاتصال العام الماضي "خدمات الوصول" يتم المتقاعدين من Office 365.</span><span class="sxs-lookup"><span data-stu-id="3e36a-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="3e36a-104">المرحلة التالية في هذه العملية سيتم إزالة "قواعد بيانات ويب الوصول إلى" استخدام قوائم SharePoint كمخزن البيانات الأساسية الخاصة بهم.</span><span class="sxs-lookup"><span data-stu-id="3e36a-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="3e36a-105">**كيف يؤثر هذا على لي؟**</span><span class="sxs-lookup"><span data-stu-id="3e36a-105">**How does this affect me?**</span></span>

<span data-ttu-id="3e36a-106">ابتداء من حزيران/يونيه عام 2019، وسوف إيقاف إنشاء قاعدة بيانات Access جديدة في SharePoint على الإنترنت وإيقاف الخدمة وأي تطبيقات المتبقية بحلول عام 2020 في نيسان/أبريل.</span><span class="sxs-lookup"><span data-stu-id="3e36a-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="3e36a-107">**ما الذي أحتاجه للتحضير لهذا التغيير؟**</span><span class="sxs-lookup"><span data-stu-id="3e36a-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="3e36a-108">ونحن نشجع إنشاء خطة انتقالية لقواعد بيانات المؤسسة الخاصة بك الوصول إلى ويب.</span><span class="sxs-lookup"><span data-stu-id="3e36a-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="3e36a-109">استخدام المسؤولين الحصول على مخزون من الوصول إلى التطبيقات التي تستخدم مواقع [SharePoint الوصول إلى تطبيق الماسح](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) .</span><span class="sxs-lookup"><span data-stu-id="3e36a-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="3e36a-110">هناك عدة طرق لترحيل بيانات قواعد بيانات Access ويب:</span><span class="sxs-lookup"><span data-stu-id="3e36a-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="3e36a-111">استيراد قاعدة البيانات وصول محلية (. ACCDB) أو إلى ملف Excel.</span><span class="sxs-lookup"><span data-stu-id="3e36a-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="3e36a-112">كما يوصي باستكشاف بوويرابس Microsoft كبديل نظاما أساسيا لإنشاء حلول الأعمال دون تعليمات برمجية للويب والأجهزة المحمولة.</span><span class="sxs-lookup"><span data-stu-id="3e36a-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>