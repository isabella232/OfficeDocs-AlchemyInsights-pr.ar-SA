---
title: تقييد SharePoint Online بالوضع الكلاسيكي
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751408"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="63735-102">تقييد SharePoint Online بالوضع الكلاسيكي</span><span class="sxs-lookup"><span data-stu-id="63735-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="63735-103">تظل بعض المؤسسات تتطلب تجربه الوضع التقليدي.</span><span class="sxs-lookup"><span data-stu-id="63735-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="63735-104">في حين انه لا توجد خطط لأزاله الوضع الكلاسيكي علي مستوي الاستخدام ، لم يعد من الممكن تقييد مؤسسه بالبالكامل (المستاجر) بالوضع الكلاسيكي للقوائم والمكتبات.</span><span class="sxs-lookup"><span data-stu-id="63735-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="63735-105">سيحصل المسؤول علي الخيارات التالية لأداره القوائم والمكتبات الفردية في الوضع الكلاسيكي باستخدام رموز التبديل الخاصة بالمشاركة المحببة التي نقدمها في المستويات التالية:</span><span class="sxs-lookup"><span data-stu-id="63735-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="63735-106">مجموعه المواقع المشتركة</span><span class="sxs-lookup"><span data-stu-id="63735-106">site collection</span></span>
- <span data-ttu-id="63735-107">مشترك</span><span class="sxs-lookup"><span data-stu-id="63735-107">site</span></span>
- <span data-ttu-id="63735-108">لائحة</span><span class="sxs-lookup"><span data-stu-id="63735-108">list</span></span>
- <span data-ttu-id="63735-109">مكتبه</span><span class="sxs-lookup"><span data-stu-id="63735-109">library</span></span>

<span data-ttu-id="63735-110">بالاضافه إلى ذلك ، فان القوائم التي تستخدم ميزات معينه وتخصيصات غير معتمده في الحالة الحديثة ستبقي تلقائيا في الوضع التقليدي.</span><span class="sxs-lookup"><span data-stu-id="63735-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="63735-111">بدءا من 1 ابريل 2019 ، سيتم بدء العملية لتعطيل المشاركة في مستوي المستاجر من القائمة الحديثة والمكتبات والاستمرار في العمل علي 31 و 2019.</span><span class="sxs-lookup"><span data-stu-id="63735-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="63735-112">سيتم تلقائيا نقل القوائم والمكتبات الموجودة في الوضع التقليدي كنتيجة للغاء الاشتراك الخاص بالمستاجر إلى الحديث.</span><span class="sxs-lookup"><span data-stu-id="63735-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="63735-113">إذا كنت بحاجه إلى الوضع الكلاسيكي ، فيرجى الاطلاع علي مزيد من المعلومات [هنا](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) وإرشادات PnP Powershell [هنا](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) التي تصف الخيارات والاداات التي يمكنك استخدامها اليوم لاستخدام تجربه الوضع التقليدي.</span><span class="sxs-lookup"><span data-stu-id="63735-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
