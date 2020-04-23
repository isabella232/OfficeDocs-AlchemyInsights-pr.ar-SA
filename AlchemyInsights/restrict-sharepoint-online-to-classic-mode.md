---
title: تقييد SharePoint Online إلى الوضع الكلاسيكي
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: c5ea5d264b62e4c349623bd431776207b38da470
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742456"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="b1f5e-102">تقييد SharePoint Online إلى الوضع الكلاسيكي</span><span class="sxs-lookup"><span data-stu-id="b1f5e-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="b1f5e-103">لا تزال بعض المؤسسات تتطلب تجربة الوضع الكلاسيكي.</span><span class="sxs-lookup"><span data-stu-id="b1f5e-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="b1f5e-104">على الرغم من عدم وجود خطط لإزالة الوضع الكلاسيكي على مستوى حبيبي، لم يعد من الممكن تقييد مؤسسة بأكملها (مستأجر) إلى الوضع الكلاسيكي للقوائم والمكتبات.</span><span class="sxs-lookup"><span data-stu-id="b1f5e-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="b1f5e-105">سيكون لدى المسؤول الخيارات التالية لإدارة القوائم الفردية والمكتبات في الوضع الكلاسيكي باستخدام مفاتيح إلغاء الاشتراك الحبيبية التي نقدمها على المستويات التالية:</span><span class="sxs-lookup"><span data-stu-id="b1f5e-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="b1f5e-106">مجموعة الموقع</span><span class="sxs-lookup"><span data-stu-id="b1f5e-106">site collection</span></span>
- <span data-ttu-id="b1f5e-107">الموقع</span><span class="sxs-lookup"><span data-stu-id="b1f5e-107">site</span></span>
- <span data-ttu-id="b1f5e-108">قائمه</span><span class="sxs-lookup"><span data-stu-id="b1f5e-108">list</span></span>
- <span data-ttu-id="b1f5e-109">مكتبه</span><span class="sxs-lookup"><span data-stu-id="b1f5e-109">library</span></span>

<span data-ttu-id="b1f5e-110">بالإضافة إلى ذلك، ستظل القوائم التي تستخدم ميزات تخصيصات معينة غير معتمدة من قبل الحديثة يتم تبديلها تلقائيًا إلى الوضع الكلاسيكي.</span><span class="sxs-lookup"><span data-stu-id="b1f5e-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="b1f5e-111">بدءًا من 1 أبريل 2019 ، ستبدأ عملية تعطيل مستوى المستأجر من القائمة الحديثة وستستمر المكتبات وتستمر حتى 31 مايو 2019.</span><span class="sxs-lookup"><span data-stu-id="b1f5e-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="b1f5e-112">سيتم تحويل القوائم والمكتبات الموجودة في الوضع الكلاسيكي نتيجة لإلغاء الاشتراك لدى المستأجر تلقائيًا إلى القوائم الحديثة.</span><span class="sxs-lookup"><span data-stu-id="b1f5e-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="b1f5e-113">إذا كنت تحتاج إلى الوضع الكلاسيكي يرجى الاطلاع على مزيد من المعلومات [هنا](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) وPnP Powershell التعليمات [هنا](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) التي تصف الخيارات والأدوات التي يمكنك استخدامها اليوم لاستخدام تجربة الوضع الكلاسيكي.</span><span class="sxs-lookup"><span data-stu-id="b1f5e-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
