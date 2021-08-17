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
ms.openlocfilehash: b53534dd0666fa64e692910aa6800abab30169a97fbe567c815ce6b948381a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057989"
---
# <a name="no-results-from-content-searchexports"></a>لا توجد نتائج من البحث/التصدير في المحتوى

قد يعود سبب المشاكل المتعلقة ببحث/تصدير المحتوى إلى عدم إرجاع أي بيانات إلى عامل تصفية أمان توافق معين تم إعداده من قبل مسؤول معين ولم يتم توصيله إلى جميع المسؤولين.

لحل هذه المشكلة، تحقق لمعرفة ما إذا كان هناك أي عوامل تصفية أمان التوافق قد تكون السبب في ذلك:
1. الاتصال إلى مركز الأمان والتوافق في Powershell
2. تشغيل الأوامر التالية:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organization $org