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
ms.openlocfilehash: 6a7c0497243ef7425917f54815e61f1244838c54
ms.sourcegitcommit: b14aa00b42ce4ca9d7dc3aa1fd57e66eae115447
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/28/2019
ms.locfileid: "30953332"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="8702e-102">تقييد SharePoint على الإنترنت إلى الوضع الكلاسيكي</span><span class="sxs-lookup"><span data-stu-id="8702e-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="8702e-103">تتطلب بعض المؤسسات لا تزال تجربة وضع التقليدية.</span><span class="sxs-lookup"><span data-stu-id="8702e-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="8702e-104">بينما لا توجد أية خطط لإزالة النمط الكلاسيكي مستوى مرغوب، بدءاً من شهر أبريل 1,2019، لم يعد الممكن لتقييد مؤسسة بأكملها (المستأجر) إلى الوضع الكلاسيكي للقوائم والمكتبات.</span><span class="sxs-lookup"><span data-stu-id="8702e-104">While there are no plans to remove classic mode at a granular level, starting April 1,2019, it will no longer be possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="8702e-105">وسيكون المسؤول الخيارات التالية لإدارة المكتبات والقوائم الفردية في الوضع الكلاسيكي استخدام رموز التبديل استبعاد الحبيبية التي نقدمها على المستويات التالية:</span><span class="sxs-lookup"><span data-stu-id="8702e-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

<span data-ttu-id="8702e-106">مكتبة-قائمة موقع مجموعة-موقع---</span><span class="sxs-lookup"><span data-stu-id="8702e-106">-- site collection -- site -- list -- library</span></span>

<span data-ttu-id="8702e-107">بالإضافة إلى ذلك، قوائم تستخدم ميزات معينة والتخصيصات التي لا يدعمها حديث سوف لا يزال يمكن تلقائياً التبديل إلى الوضع الكلاسيكي.</span><span class="sxs-lookup"><span data-stu-id="8702e-107">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="8702e-108">بعد 1 نيسان/أبريل، القوائم والمكتبات الموجودة في الوضع التقليدي نتيجة للمستأجر الخروج تلقائياً إدارة على مستوى الموقع ومستوى القائمة.</span><span class="sxs-lookup"><span data-stu-id="8702e-108">After April 1, lists and libraries that are in classic mode as a result of tenant opt-out will automatically be managed at the site level and list level.</span></span>

<span data-ttu-id="8702e-109">إذا تطلب الوضع الكلاسيكي يرجى الاطلاع على مزيد من المعلومات هنا وتعليمه PnP Powershell هنا يصف خيارات وأدوات يمكنك استخدامها اليوم للإعداد لإزالة المستأجر مستوى الخروج في 1 نيسان/أبريل.</span><span class="sxs-lookup"><span data-stu-id="8702e-109">If you require classic mode please see more information here and PnP Powershell instruction here that describes options and tools you can use today to prepare for the removal of the tenant level opt-out on April 1.</span></span>
