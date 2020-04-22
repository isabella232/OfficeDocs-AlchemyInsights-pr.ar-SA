---
title: التقاعد خدمات الوصول
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 977bd5887ef58b328463a9befcd6b47ac55f5a85
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687245"
---
# <a name="access-services-retirement"></a>التقاعد خدمات الوصول

كما أعلنا في الأصل في MC97576 ، في مارس 2017 ، واستمرنا في التواصل على مدار العام الماضي يتم سحب خدمات Access. المرحلة التالية في هذه العملية ستكون إزالة قواعد بيانات ويب Access التي تستخدم قوائم SharePoint كتخزين البيانات الأساسية الخاصة بهم.

**كيف يؤثر هذا علي؟**

بدءًا من يونيو 2019 ، سنتوقف عن إنشاء قواعد بيانات Access جديدة في SharePoint Online ونغلق الخدمة وأي تطبيقات متبقية بحلول أبريل 2020.

**ما الذي يجب علي فعله للتحضير لهذا التغيير؟**

نحن نشجعك على إنشاء خطة انتقالية لقواعد بيانات الويب Access الخاصة بمؤسستك. يمكن للمسؤولين استخدام [ماسح تطبيق SharePoint Access للحصول](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) على مخزون من تطبيقات Access التي تستخدمها المواقع.

هناك عدة طرق لترحيل بيانات قواعد بيانات ويب Access:

- الاستيراد إلى قاعدة بيانات Access المحلية (. ACCDB) أو إلى ملف Excel.
- نوصي أيضًا باستكشاف Microsoft PowerApps كمنصة بديلة لإنشاء حلول أعمال بدون رمز لأجهزة الويب والأجهزة المحمولة.