---
title: لا يوجد نتائج البحث المحتوى
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800154"
---
# <a name="no-results-from-content-searchexports"></a>لا توجد نتائج من محتوى البحث/الصادرات

مشاكل مع محتوى البحث/الصادرات عدم إرجاع أية بيانات قد يرجع إلى "تصفية الأمان توافق" معين تم إعداد إدارة معينة وعدم إبلاغه إلى جميع المسؤولين.

لحل هذه المشكلة، تحقق من عدم وجود أي "عوامل تصفية أمان التوافق" الذي يمكن أن يسبب هذا:
1. الاتصال بأمان و Powershell مركز التوافق
2. قم بتشغيل كوماندليتس التالية:
<br>$org = "yourdomain.com"
<br>الحصول على كومبليانسيسيكوريتيفيلتير-مؤسسة $org