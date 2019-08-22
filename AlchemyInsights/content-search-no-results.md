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
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516766"
---
# <a name="no-results-from-content-searchexports"></a>لا توجد نتائج من محتوى البحث/الصادرات

مشاكل مع محتوى البحث/الصادرات عدم إرجاع أية بيانات قد يرجع إلى "تصفية الأمان توافق" معين تم إعداد إدارة معينة وعدم إبلاغه إلى جميع المسؤولين.

لحل هذه المشكلة، تحقق من عدم وجود أي "عوامل تصفية أمان التوافق" الذي يمكن أن يسبب هذا:
1. الاتصال بأمان و Powershell مركز التوافق
2. قم بتشغيل كوماندليتس التالية:
<br>$org = "yourdomain.com"
<br>الحصول على كومبليانسيسيكوريتيفيلتير-مؤسسة $org