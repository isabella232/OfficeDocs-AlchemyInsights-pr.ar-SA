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
ms.openlocfilehash: c51e48fe5694f964aef74c2973f774b44415ebb8
ms.sourcegitcommit: 21cfb213183188d32a3743f66db10a8463019965
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/28/2019
ms.locfileid: "30955963"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="4c5d3-102">تقييد SharePoint على الإنترنت إلى الوضع الكلاسيكي</span><span class="sxs-lookup"><span data-stu-id="4c5d3-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="4c5d3-103">تتطلب بعض المؤسسات لا تزال تجربة وضع التقليدية.</span><span class="sxs-lookup"><span data-stu-id="4c5d3-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="4c5d3-104">بينما لا توجد أية خطط لإزالة النمط الكلاسيكي مستوى مرغوب، بدءاً من شهر أبريل 1,2019، لم يعد الممكن لتقييد مؤسسة بأكملها (المستأجر) إلى الوضع الكلاسيكي للقوائم والمكتبات.</span><span class="sxs-lookup"><span data-stu-id="4c5d3-104">While there are no plans to remove classic mode at a granular level, starting April 1,2019, it will no longer be possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="4c5d3-105">وسيكون المسؤول الخيارات التالية لإدارة المكتبات والقوائم الفردية في الوضع الكلاسيكي استخدام رموز التبديل استبعاد الحبيبية التي نقدمها على المستويات التالية:</span><span class="sxs-lookup"><span data-stu-id="4c5d3-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="4c5d3-106">مجموعة الموقع</span><span class="sxs-lookup"><span data-stu-id="4c5d3-106">site collection</span></span>
- <span data-ttu-id="4c5d3-107">موقع</span><span class="sxs-lookup"><span data-stu-id="4c5d3-107">site</span></span>
- <span data-ttu-id="4c5d3-108">قائمة</span><span class="sxs-lookup"><span data-stu-id="4c5d3-108">list</span></span>
- <span data-ttu-id="4c5d3-109">مكتبة</span><span class="sxs-lookup"><span data-stu-id="4c5d3-109">library</span></span>

<span data-ttu-id="4c5d3-110">بالإضافة إلى ذلك، قوائم تستخدم ميزات معينة والتخصيصات التي لا يدعمها حديث سوف لا يزال يمكن تلقائياً التبديل إلى الوضع الكلاسيكي.</span><span class="sxs-lookup"><span data-stu-id="4c5d3-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="4c5d3-111">بعد 1 نيسان/أبريل، القوائم والمكتبات الموجودة في الوضع التقليدي نتيجة للمستأجر الخروج تلقائياً إدارة على مستوى الموقع ومستوى القائمة.</span><span class="sxs-lookup"><span data-stu-id="4c5d3-111">After April 1, lists and libraries that are in classic mode as a result of tenant opt-out will automatically be managed at the site level and list level.</span></span>

<span data-ttu-id="4c5d3-112">إذا تطلب الوضع الكلاسيكي يرجى الاطلاع على مزيد من المعلومات هنا وتعليمه PnP Powershell هنا يصف خيارات وأدوات يمكنك استخدامها اليوم للإعداد لإزالة المستأجر مستوى الخروج في 1 نيسان/أبريل.</span><span class="sxs-lookup"><span data-stu-id="4c5d3-112">If you require classic mode please see more information here and PnP Powershell instruction here that describes options and tools you can use today to prepare for the removal of the tenant level opt-out on April 1.</span></span>
