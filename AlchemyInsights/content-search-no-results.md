---
title: لا توجد نتائج في البحث عن المحتوي
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680634"
---
# <a name="no-results-from-content-searchexports"></a>لا توجد نتائج من البحث في المحتوي/التصديرات

المشاكل المتعلقة بالبحث في المحتوي/عمليات التصدير لا يتم إرجاع اي بيانات بسبب عامل تصفيه أمان توافق معين تم اعداده من قبل مسؤول معين ولا يتم الاتصال به لجميع المسؤولين.

لحل هذه المشكلة ، تحقق لمعرفه ما إذا كانت هناك اي عوامل تصفيه أمان للتوافق قد تؤدي إلى ذلك:
1. الاتصال بمركز التوافق والأمان Powershell
2. قم بتشغيل الكوماندليتس التالية:
<br>$org = "yourdomain.com"
<br>كومبليانسيسيكوريتيفيلتير-مؤسسه $org