---
title: حول تحديثات أمان Exchange Server
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005482"
- "9005483"
- "9413"
- "9412"
ms.openlocfilehash: 87a5cf1ac4dfb96a5406f6b1431adb6ead074fd6
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "50480848"
---
# <a name="about-exchange-server-security-updates"></a><span data-ttu-id="0a15d-102">حول تحديثات أمان Exchange Server</span><span class="sxs-lookup"><span data-stu-id="0a15d-102">About Exchange Server Security updates</span></span>

<span data-ttu-id="0a15d-103">أصدرت Microsoft سلسلة من تحديثات الأمان الهامة ل Exchange Server في الموقع الداخلي.</span><span class="sxs-lookup"><span data-stu-id="0a15d-103">Microsoft has released a series of critical security updates for Exchange Server on-premises.</span></span> <span data-ttu-id="0a15d-104">إصدارات الخادم المتأثرة هي أي مستويات تحديث ل Exchange Server 2010 و2013 و2016 و2019.</span><span class="sxs-lookup"><span data-stu-id="0a15d-104">The affected server versions are any update levels of Exchange Server 2010, 2013, 2016 and 2019.</span></span> <span data-ttu-id="0a15d-105">لا يؤثر Exchange Online، ولكن إذا كان لديك بعض خوادم Exchange في الموقع بسبب التكوين المختلط، فمن المحتمل أن تكون عرضة للتأثر.</span><span class="sxs-lookup"><span data-stu-id="0a15d-105">Exchange Online is NOT impacted, but if you have some on-premises Exchange servers due to Hybrid configuration, they are potentially vulnerable.</span></span>

<span data-ttu-id="0a15d-106">لتحديث الخوادم في الموقع، يجب تشغيل الإصدارات التالية من Exchange على الأقل:</span><span class="sxs-lookup"><span data-stu-id="0a15d-106">To update your on-premises servers will have to be running at least the following versions of Exchange:</span></span>

- <span data-ttu-id="0a15d-107">Exchange 2010 Service Pack 3</span><span class="sxs-lookup"><span data-stu-id="0a15d-107">Exchange 2010 Service Pack 3</span></span>
- <span data-ttu-id="0a15d-108">Exchange Server 2013 CU 23</span><span class="sxs-lookup"><span data-stu-id="0a15d-108">Exchange Server 2013 CU 23</span></span>
- <span data-ttu-id="0a15d-109">Exchange Server 2016 CU 19 أو CU 18</span><span class="sxs-lookup"><span data-stu-id="0a15d-109">Exchange Server 2016 CU 19 or CU 18</span></span>
- <span data-ttu-id="0a15d-110">Exchange Server 2019 CU 8 أو CU 7</span><span class="sxs-lookup"><span data-stu-id="0a15d-110">Exchange Server 2019 CU 8 or CU 7</span></span>

<span data-ttu-id="0a15d-111">الرجاء الاطلاع على الإعلان التالي لتحديد موقع الإصلاحات: تم إصداره: تحديثات أمان [Exchange Server في مارس 2021](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)</span><span class="sxs-lookup"><span data-stu-id="0a15d-111">Please see the following announcement for location of fixes: [Released: March 2021 Exchange Server Security Updates](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)</span></span>

<span data-ttu-id="0a15d-112">**ملاحظات مهمة:**</span><span class="sxs-lookup"><span data-stu-id="0a15d-112">**Important notes:**</span></span>

<span data-ttu-id="0a15d-113">لن يعمل تثبيت التحديثات إذا كانت الخوادم في الموقع لا تعمل إصدارات Exchange المطلوبة، كما هو محدث في القائمة أعلاه.</span><span class="sxs-lookup"><span data-stu-id="0a15d-113">Installation of updates will not work if your on-premises servers are not running required Exchange versions, as per the above list.</span></span>

<span data-ttu-id="0a15d-114">إذا تم تثبيت التحديثات يدويا، فالرجاء قراءة القسم "المشاكل المعروفة" في مقالات تحديث KB للحصول على معلومات مهمة.</span><span class="sxs-lookup"><span data-stu-id="0a15d-114">If installing updates manually, please read the "Known issues" section of update KB articles for important information.</span></span> <span data-ttu-id="0a15d-115">يجب تشغيل تحديثات الأمان من مطالبة CMD/PowerShell مرتفعة!</span><span class="sxs-lookup"><span data-stu-id="0a15d-115">Security updates MUST be run from elevated CMD/PowerShell prompt!</span></span>
