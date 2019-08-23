---
title: تقييد SharePoint على الإنترنت إلى الوضع الكلاسيكي
ms.author: kirks
author: Techwriter40
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
ms.openlocfilehash: e7ecfd8c2f1a532355bfb8c2c0a846fc0d6e88b1
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551546"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="279eb-102">تقييد SharePoint على الإنترنت إلى الوضع الكلاسيكي</span><span class="sxs-lookup"><span data-stu-id="279eb-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="279eb-103">تتطلب بعض المؤسسات لا تزال تجربة وضع التقليدية.</span><span class="sxs-lookup"><span data-stu-id="279eb-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="279eb-104">بينما لا توجد أية خطط لإزالة النمط الكلاسيكي مستوى مرغوب، يعد المحتملة لتقييد مؤسسة (المستأجر) إلى الوضع الكلاسيكي للقوائم والمكتبات.</span><span class="sxs-lookup"><span data-stu-id="279eb-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="279eb-105">وسيكون المسؤول الخيارات التالية لإدارة المكتبات والقوائم الفردية في الوضع الكلاسيكي استخدام رموز التبديل استبعاد الحبيبية التي نقدمها على المستويات التالية:</span><span class="sxs-lookup"><span data-stu-id="279eb-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="279eb-106">مجموعة الموقع</span><span class="sxs-lookup"><span data-stu-id="279eb-106">site collection</span></span>
- <span data-ttu-id="279eb-107">موقع</span><span class="sxs-lookup"><span data-stu-id="279eb-107">site</span></span>
- <span data-ttu-id="279eb-108">قائمة</span><span class="sxs-lookup"><span data-stu-id="279eb-108">list</span></span>
- <span data-ttu-id="279eb-109">مكتبة</span><span class="sxs-lookup"><span data-stu-id="279eb-109">library</span></span>

<span data-ttu-id="279eb-110">بالإضافة إلى ذلك، قوائم تستخدم ميزات معينة والتخصيصات التي لا يدعمها حديث سوف لا يزال يمكن تلقائياً التبديل إلى الوضع الكلاسيكي.</span><span class="sxs-lookup"><span data-stu-id="279eb-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="279eb-111">ابتداء من نيسان/أبريل 1، 2019، عملية لتعطيل مستوى المستأجر الانسحاب من قائمة حديثة وسوف ابدأ المكتبات وتستمر حتى 31 مايو عام 2019.</span><span class="sxs-lookup"><span data-stu-id="279eb-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="279eb-112">سيتم تلقائياً نقل القوائم والمكتبات الموجودة في الوضع التقليدي نتيجة للمستأجر استبعاد الحديثة.</span><span class="sxs-lookup"><span data-stu-id="279eb-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="279eb-113">إذا تطلب الوضع الكلاسيكي مزيد من المعلومات انظر [هنا](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) وتعليمه PnP Powershell [هنا](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) يصف الخيارات والأدوات التي يمكنك استخدامها اليوم على الاستعانة بخبرة الوضع الكلاسيكي.</span><span class="sxs-lookup"><span data-stu-id="279eb-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
