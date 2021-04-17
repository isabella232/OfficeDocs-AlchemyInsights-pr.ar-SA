---
title: البحث في المحتوى بلا نتائج
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
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816835"
---
# <a name="no-results-from-content-searchexports"></a>لا توجد نتائج من البحث/التصدير في المحتوى

قد يعود سبب المشاكل المتعلقة ببحث/تصدير المحتوى إلى عدم إرجاع أي بيانات إلى عامل تصفية أمان توافق معين تم إعداده من قبل مسؤول معين ولم يتم توصيله إلى جميع المسؤولين.

لحل هذه المشكلة، تحقق لمعرفة ما إذا كان هناك أي عوامل تصفية أمان التوافق قد تكون السبب في ذلك:
1. الاتصال بمركز الأمان والتوافق في Powershell
2. تشغيل الأوامر التالية:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organization $org