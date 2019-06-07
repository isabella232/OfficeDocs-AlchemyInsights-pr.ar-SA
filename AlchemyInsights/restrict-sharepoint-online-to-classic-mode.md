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
ms.openlocfilehash: 76f0b5ed67d3220559d25dfd72c7535181a4513b
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761746"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="1fb21-102">تقييد SharePoint على الإنترنت إلى الوضع الكلاسيكي</span><span class="sxs-lookup"><span data-stu-id="1fb21-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="1fb21-103">تتطلب بعض المؤسسات لا تزال تجربة وضع التقليدية.</span><span class="sxs-lookup"><span data-stu-id="1fb21-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="1fb21-104">بينما لا توجد أية خطط لإزالة النمط الكلاسيكي مستوى مرغوب، يعد المحتملة لتقييد مؤسسة (المستأجر) إلى الوضع الكلاسيكي للقوائم والمكتبات.</span><span class="sxs-lookup"><span data-stu-id="1fb21-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="1fb21-105">وسيكون المسؤول الخيارات التالية لإدارة المكتبات والقوائم الفردية في الوضع الكلاسيكي استخدام رموز التبديل استبعاد الحبيبية التي نقدمها على المستويات التالية:</span><span class="sxs-lookup"><span data-stu-id="1fb21-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="1fb21-106">مجموعة الموقع</span><span class="sxs-lookup"><span data-stu-id="1fb21-106">site collection</span></span>
- <span data-ttu-id="1fb21-107">موقع</span><span class="sxs-lookup"><span data-stu-id="1fb21-107">site</span></span>
- <span data-ttu-id="1fb21-108">قائمة</span><span class="sxs-lookup"><span data-stu-id="1fb21-108">list</span></span>
- <span data-ttu-id="1fb21-109">مكتبة</span><span class="sxs-lookup"><span data-stu-id="1fb21-109">library</span></span>

<span data-ttu-id="1fb21-110">بالإضافة إلى ذلك، قوائم تستخدم ميزات معينة والتخصيصات التي لا يدعمها حديث سوف لا يزال يمكن تلقائياً التبديل إلى الوضع الكلاسيكي.</span><span class="sxs-lookup"><span data-stu-id="1fb21-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="1fb21-111">ابتداء من نيسان/أبريل 1، 2019، عملية لتعطيل مستوى المستأجر الانسحاب من قائمة حديثة وسوف ابدأ المكتبات وتستمر حتى 31 مايو عام 2019.</span><span class="sxs-lookup"><span data-stu-id="1fb21-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="1fb21-112">سيتم تلقائياً نقل القوائم والمكتبات الموجودة في الوضع التقليدي نتيجة للمستأجر استبعاد الحديثة.</span><span class="sxs-lookup"><span data-stu-id="1fb21-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="1fb21-113">إذا تطلب الوضع الكلاسيكي مزيد من المعلومات انظر [هنا](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) وتعليمه PnP Powershell [هنا](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) يصف الخيارات والأدوات التي يمكنك استخدامها اليوم على الاستعانة بخبرة الوضع الكلاسيكي.</span><span class="sxs-lookup"><span data-stu-id="1fb21-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
