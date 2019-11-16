---
title: الوصول إلى خدمات التقاعد
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 197366882468ebc87fc26f2fe2733371790d1871
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/15/2019
ms.locfileid: "36747771"
---
# <a name="access-services-retirement"></a>الوصول إلى خدمات التقاعد

وكما اعلنا في الأصل في MC97576 ، في آذار/مارس 2017 ، وواصلنا التواصل علي مدي السنه الماضية ويجري تقاعد خدمات الوصول من مكتب 365. ستكون المرحلة التالية في هذه العملية أزاله قواعد بيانات ويب Access التي تستخدم قوائم SharePoint كتخزين البيانات الاساسيه الخاصة بهم.

**كيف يؤثر هذا علي ؟**

بدءا يونيو 2019 ، سوف نتوقف عن إنشاء قواعد بيانات Access جديده في SharePoint علي الإنترنت وإيقاف تشغيل الخدمة وآيه تطبيقات المتبقية بحلول ابريل 2020.

**ما الذي يجب علي القيام به للتحضير لهذا التغيير ؟**

نحن نشجعك علي إنشاء خطه انتقاليه لقواعد بيانات الوصول إلى الويب الخاصة بمؤسسك. يمكن للمشرفين استخدام [الماسح الضوئي لتطبيق SharePoint access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) للحصول علي مخزون من تطبيقات access التي تستخدمها المواقع.

هناك العديد من الطرق لترحيل البيانات "الوصول إلى قواعد ويب":

- الاستيراد إلى قاعده بيانات Access محليه (. ACCDB) أو إلى ملف Excel.
- نوصي أيضا باستكشاف Microsoft PowerApps كنظام أساسي بديل لإنشاء حلول عمل بدون تعليمات برمجيه لأجهزه الويب والجوال.