---
title: التقاعد في Access services
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698633"
---
# <a name="access-services-retirement"></a>التقاعد في Access services

بما اننا إعلاننا بالفعل في MC97576 ، وفي مارس 2017 ، ومستمر للتواصل عبر السنه الماضية ، سيتم إيقاف خدمه Access. ستكون المرحلة التالية في هذه العملية هي أزاله قواعد بيانات Access علي ويب التي تستخدم قوائم SharePoint كمساحة تخزين البيانات الاساسيه الخاصة بها.

**كيف يؤثر هذا ؟**

بدءا من يونيو 2019 ، سنقوم بإيقاف إنشاء قواعد بيانات Access جديده في SharePoint Online وإيقاف تشغيل الخدمة وأي تطبيقات متبقية بحلول ابريل 2020.

**ما الذي احتاج إلى فعله للتحضير لهذا التغيير ؟**

نحن نشجعك علي إنشاء خطه انتقال لقواعد بيانات Access علي ويب الخاصة بمؤسسك. يمكن للمسؤولين استخدام [ماسح تطبيق SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) للحصول علي مخزون تطبيقات Access التي تستخدمها المواقع.

هناك طرق متعددة لترحيل بيانات قواعد بيانات Access علي الويب:

- الاستيراد إلى قاعده بيانات Access محليه (. ACCDB) أو إلى ملف Excel.
- نوصي أيضا باستكشاف Microsoft PowerApps كنظام أساسي بديل لإنشاء حلول للشركات التي لا تستخدم التعليمات البرمجية للاجهزه المحمولة والويب.