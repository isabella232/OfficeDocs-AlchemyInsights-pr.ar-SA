---
title: الوصول إلى خدمات التقاعد
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 395dac6abf1562aa0da0b1d87eddd943affefc3f
ms.sourcegitcommit: b2c9202b94fa1ce73dbeb3e43b219ba07e46e7e3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/14/2019
ms.locfileid: "33973894"
---
# <a name="access-services-retirement"></a><span data-ttu-id="9cded-102">الوصول إلى خدمات التقاعد</span><span class="sxs-lookup"><span data-stu-id="9cded-102">Access services retirement</span></span>

<span data-ttu-id="9cded-103">ونحن أصلاً في MC97576، وأعلن في آذار/مارس عام 2017، وتواصل الاتصال العام الماضي "خدمات الوصول" يتم المتقاعدين من Office 365.</span><span class="sxs-lookup"><span data-stu-id="9cded-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="9cded-104">المرحلة التالية في هذه العملية سيتم إزالة "قواعد بيانات ويب الوصول إلى" استخدام قوائم SharePoint كمخزن البيانات الأساسية الخاصة بهم.</span><span class="sxs-lookup"><span data-stu-id="9cded-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

## <a name="how-does-this-affect-me"></a><span data-ttu-id="9cded-105">كيف يؤثر هذا على لي؟</span><span class="sxs-lookup"><span data-stu-id="9cded-105">How does this affect me?</span></span>

<span data-ttu-id="9cded-106">ابتداء من حزيران/يونيه عام 2019، وسوف إيقاف إنشاء قاعدة بيانات Access جديدة في SharePoint على الإنترنت وإيقاف الخدمة وأي تطبيقات المتبقية بحلول عام 2020 في نيسان/أبريل.</span><span class="sxs-lookup"><span data-stu-id="9cded-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

## <a name="what-do-i-need-to-do-to-prepare-for-this-change"></a><span data-ttu-id="9cded-107">ما الذي أحتاجه للتحضير لهذا التغيير؟</span><span class="sxs-lookup"><span data-stu-id="9cded-107">What do I need to do to prepare for this change?</span></span>

<span data-ttu-id="9cded-108">ونحن نشجع إنشاء خطة انتقالية لقواعد بيانات المؤسسة الخاصة بك الوصول إلى ويب.</span><span class="sxs-lookup"><span data-stu-id="9cded-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="9cded-109">استخدام المسؤولين الحصول على مخزون من الوصول إلى التطبيقات التي تستخدم مواقع [SharePoint الوصول إلى تطبيق الماسح](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) .</span><span class="sxs-lookup"><span data-stu-id="9cded-109">Admins can use the [SharePoint Access app scanner](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) to obtain an inventory of the Access apps that sites are using.</span></span> 

<span data-ttu-id="9cded-110">هناك عدة طرق لترحيل بيانات قواعد بيانات Access ويب:</span><span class="sxs-lookup"><span data-stu-id="9cded-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="9cded-111">استيراد قاعدة البيانات وصول محلية (. ACCDB) أو إلى ملف Excel.</span><span class="sxs-lookup"><span data-stu-id="9cded-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="9cded-112">كما يوصي باستكشاف بوويرابس Microsoft كبديل نظاما أساسيا لإنشاء حلول الأعمال دون تعليمات برمجية للويب والأجهزة المحمولة.</span><span class="sxs-lookup"><span data-stu-id="9cded-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>