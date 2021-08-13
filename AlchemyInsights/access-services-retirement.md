---
title: تقاعد خدمات Access
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
ms.openlocfilehash: 32da879de230dc0ed99563ad881ab5b2479b8453933a127961a26d619e108ab9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938682"
---
# <a name="access-services-retirement"></a>تقاعد خدمات Access

كما أعلنا في الأصل في MC97576، في مارس 2017، وتابعنا التواصل خلال السنة الماضية Access Services يتم الآن Access Services العمل. ستكون المرحلة التالية في هذه العملية إزالة قواعد بيانات Access على ويب التي تستخدم SharePoint كمساحة تخزين البيانات الأساسية الخاصة بها.

**كيف يؤثر ذلك علي؟**

اعتبارا من يونيو 2019، سنتوقف عن إنشاء قواعد بيانات Access جديدة في SharePoint Online ونوقف تشغيل الخدمة وأي تطبيقات متبقة بحلول أبريل 2020.

**ما الذي أحتاج إليه للتحضير لهذا التغيير؟**

إننا نشجعك على إنشاء خطة انتقال لقواعد بيانات Access على الويب الخاصة مؤسستك. يمكن للمسؤولين استخدام ماسح [SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) للحصول على مخزون لتطبيقات Access التي تستخدمها المواقع.

هناك عدة طرق لترحيل بيانات قواعد بيانات Access على الويب:

- الاستيراد إلى قاعدة بيانات Access محلية (. ACCDB) أو إلى Excel ملف.
- نوصي أيضا باستكشاف Microsoft PowerApps كنهاية بديلة لإنشاء حلول أعمال بدون تعليمات برمجية للأجهزة المحمولة والويب.