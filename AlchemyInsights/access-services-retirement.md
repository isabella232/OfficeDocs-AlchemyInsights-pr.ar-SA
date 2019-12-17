---
title: الوصول إلى خدمات التقاعد
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: cb8123583b68e945ef878fdbaf211fd1d8205bb3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050476"
---
# <a name="access-services-retirement"></a><span data-ttu-id="63aa9-102">الوصول إلى خدمات التقاعد</span><span class="sxs-lookup"><span data-stu-id="63aa9-102">Access services retirement</span></span>

<span data-ttu-id="63aa9-103">وكما اعلنا في الأصل في MC97576 ، في آذار/مارس 2017 ، وواصلنا التواصل علي مدي السنه الماضية ويجري تقاعد خدمات الوصول من مكتب 365.</span><span class="sxs-lookup"><span data-stu-id="63aa9-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="63aa9-104">ستكون المرحلة التالية في هذه العملية أزاله قواعد بيانات ويب Access التي تستخدم قوائم SharePoint كتخزين البيانات الاساسيه الخاصة بهم.</span><span class="sxs-lookup"><span data-stu-id="63aa9-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="63aa9-105">**كيف يؤثر هذا علي ؟**</span><span class="sxs-lookup"><span data-stu-id="63aa9-105">**How does this affect me?**</span></span>

<span data-ttu-id="63aa9-106">بدءا يونيو 2019 ، سوف نتوقف عن إنشاء قواعد بيانات Access جديده في SharePoint علي الإنترنت وإيقاف تشغيل الخدمة وآيه تطبيقات المتبقية بحلول ابريل 2020.</span><span class="sxs-lookup"><span data-stu-id="63aa9-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="63aa9-107">**ما الذي يجب علي القيام به للتحضير لهذا التغيير ؟**</span><span class="sxs-lookup"><span data-stu-id="63aa9-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="63aa9-108">نحن نشجعك علي إنشاء خطه انتقاليه لقواعد بيانات الوصول إلى الويب الخاصة بمؤسسك.</span><span class="sxs-lookup"><span data-stu-id="63aa9-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="63aa9-109">يمكن للمشرفين استخدام [الماسح الضوئي لتطبيق SharePoint access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) للحصول علي مخزون من تطبيقات access التي تستخدمها المواقع.</span><span class="sxs-lookup"><span data-stu-id="63aa9-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="63aa9-110">هناك العديد من الطرق لترحيل البيانات "الوصول إلى قواعد ويب":</span><span class="sxs-lookup"><span data-stu-id="63aa9-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="63aa9-111">الاستيراد إلى قاعده بيانات Access محليه (. ACCDB) أو إلى ملف Excel.</span><span class="sxs-lookup"><span data-stu-id="63aa9-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="63aa9-112">نوصي أيضا باستكشاف Microsoft PowerApps كنظام أساسي بديل لإنشاء حلول عمل بدون تعليمات برمجيه لأجهزه الويب والجوال.</span><span class="sxs-lookup"><span data-stu-id="63aa9-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>