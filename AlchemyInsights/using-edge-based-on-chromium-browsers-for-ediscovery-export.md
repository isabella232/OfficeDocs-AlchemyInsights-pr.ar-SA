---
title: استخدام Microsoft Edge استنادا إلى مستعرضات Chromium لتصدير Ediscovery
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3473"
- "3100022"
ms.openlocfilehash: 7ee724e5109effce8883be50e360948313c84b34
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834358"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a><span data-ttu-id="016e1-102">استخدام Microsoft Edge استنادا إلى مستعرضات Chromium لتصدير Ediscovery</span><span class="sxs-lookup"><span data-stu-id="016e1-102">Using Microsoft Edge based on Chromium browsers for Ediscovery export</span></span>

<span data-ttu-id="016e1-103">بسبب التغيير الأخير، لن يتم تمكين دعم ClickOnce في مستعرضات Microsoft Edge بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="016e1-103">Due to a recent change, Microsoft Edge browsers will no longer have ClickOnce support enabled by default.</span></span> <span data-ttu-id="016e1-104">لمواصلة استخدام أداة تصدير eDiscovery ل Microsoft 365، ستحتاج إما إلى استخدام Microsoft Internet Explorer أو تمكين دعم ClickOnce في Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="016e1-104">To continue using the Microsoft 365 eDiscovery Export Tool, you will either need to use Microsoft Internet Explorer or enable ClickOnce Support in Microsoft Edge.</span></span> 

<span data-ttu-id="016e1-105">لتمكين دعم ClickOnce في Microsoft Edge استنادا إلى Chromium:</span><span class="sxs-lookup"><span data-stu-id="016e1-105">To enable ClickOnce Support in Microsoft Edge based on Chromium:</span></span> 
1. <span data-ttu-id="016e1-106">في مستعرض Microsoft Edge، تفضل بزيارة edge://flags/#edge-click-once.</span><span class="sxs-lookup"><span data-stu-id="016e1-106">In your Microsoft Edge browser, visit edge://flags/#edge-click-once.</span></span>
2. <span data-ttu-id="016e1-107">بالنسبة إلى خيار دعم ClickOnce، قم بتغيير القيمة من **افتراضي** أو **معطل** إلى **تمكين**.</span><span class="sxs-lookup"><span data-stu-id="016e1-107">For the ClickOnce Support option, change the value from **Default** or **Disabled** to **Enabled**.</span></span> 
3. <span data-ttu-id="016e1-108">في أسفل نافذة المستعرض، حدد **إعادة تشغيل**.</span><span class="sxs-lookup"><span data-stu-id="016e1-108">At the bottom of the browser window, select **Restart**.</span></span> <br>
 <span data-ttu-id="016e1-109">سيتغير هذا التغيير بعد إعادة تشغيل Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="016e1-109">The change will take effect after restarting Microsoft Edge.</span></span> 

<span data-ttu-id="016e1-110">للحصول على معلومات حول هذا الموضوع والخطوات المتعلقة بتثبيت أداة التصدير، راجع: [ تصدير نتائج البحث في المحتوى](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="016e1-110">For information on this and steps for installing the  export tool, see: [ Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>