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
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a>استخدام Microsoft Edge استنادا إلى مستعرضات Chromium لتصدير Ediscovery

بسبب التغيير الأخير، لن يتم تمكين دعم ClickOnce في مستعرضات Microsoft Edge بشكل افتراضي. لمواصلة استخدام أداة تصدير eDiscovery ل Microsoft 365، ستحتاج إما إلى استخدام Microsoft Internet Explorer أو تمكين دعم ClickOnce في Microsoft Edge. 

لتمكين دعم ClickOnce في Microsoft Edge استنادا إلى Chromium: 
1. في مستعرض Microsoft Edge، تفضل بزيارة edge://flags/#edge-click-once.
2. بالنسبة إلى خيار دعم ClickOnce، قم بتغيير القيمة من **افتراضي** أو **معطل** إلى **تمكين**. 
3. في أسفل نافذة المستعرض، حدد **إعادة تشغيل**. <br>
 سيتغير هذا التغيير بعد إعادة تشغيل Microsoft Edge. 

للحصول على معلومات حول هذا الموضوع والخطوات المتعلقة بتثبيت أداة التصدير، راجع: [ تصدير نتائج البحث في المحتوى](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).