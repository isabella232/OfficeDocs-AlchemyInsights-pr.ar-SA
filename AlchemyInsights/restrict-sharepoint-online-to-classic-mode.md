---
title: تقييد SharePoint علي الإنترنت إلى الوضع الكلاسيكي
ms.author: pebaum
author: pebaum
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: b58a1c3fc331c739080542917d8945c090ec0d94
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048747"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="3b8c5-102">تقييد SharePoint علي الإنترنت إلى الوضع الكلاسيكي</span><span class="sxs-lookup"><span data-stu-id="3b8c5-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="3b8c5-103">بعض المؤسسات لا تزال تتطلب تجربه الوضع الكلاسيكي.</span><span class="sxs-lookup"><span data-stu-id="3b8c5-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="3b8c5-104">في حين لا توجد خطط لأزاله الوضع الكلاسيكي علي مستوي الحبيبية ، لم يعد من الممكن تقييد مؤسسه بأكملها (المستاجر) إلى الوضع الكلاسيكي للقوائم والمكتبات.</span><span class="sxs-lookup"><span data-stu-id="3b8c5-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="3b8c5-105">سيكون لدي المشرف الخيارات التالية لأداره القوائم الفردية والمكتبات في الوضع الكلاسيكي باستخدام رموز تبديل الانسحاب المحببة التي نوفرها علي المستويات التالية:</span><span class="sxs-lookup"><span data-stu-id="3b8c5-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="3b8c5-106">مجموعه الموقع</span><span class="sxs-lookup"><span data-stu-id="3b8c5-106">site collection</span></span>
- <span data-ttu-id="3b8c5-107">الموقع</span><span class="sxs-lookup"><span data-stu-id="3b8c5-107">site</span></span>
- <span data-ttu-id="3b8c5-108">قائمه</span><span class="sxs-lookup"><span data-stu-id="3b8c5-108">list</span></span>
- <span data-ttu-id="3b8c5-109">مكتبه</span><span class="sxs-lookup"><span data-stu-id="3b8c5-109">library</span></span>

<span data-ttu-id="3b8c5-110">بالاضافه إلى ذلك ، القوائم التي تستخدم ميزات معينه والتخصيصات التي لا تدعمها الحديثة سوف لا تزال تحول تلقائيا إلى الوضع الكلاسيكي.</span><span class="sxs-lookup"><span data-stu-id="3b8c5-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="3b8c5-111">ابتداء من 1 ابريل 2019 ، وعمليه لتعطيل مستوي المستاجر الانسحاب من القائمة الحديثة والمكتبات سوف تبدا وتستمر حتى 31 مايو ، 2019.</span><span class="sxs-lookup"><span data-stu-id="3b8c5-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="3b8c5-112">سيتم تلقائيا تحويل القوائم والمكتبات الموجودة في الوضع الكلاسيكي كنتيجة للغاء اشتراك المستاجر إلى حديثه.</span><span class="sxs-lookup"><span data-stu-id="3b8c5-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="3b8c5-113">إذا كنت تحتاج إلى الوضع الكلاسيكي الرجاء الاطلاع علي مزيد من المعلومات [هنا](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) وتعليمات Powershell PnP [هنا](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) التي تصف الخيارات والاداات التي يمكنك استخدامها اليوم لاستخدام تجربه الوضع الكلاسيكي.</span><span class="sxs-lookup"><span data-stu-id="3b8c5-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
