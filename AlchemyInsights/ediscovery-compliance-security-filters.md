---
title: لم يتم إرجاع اي نتائج اثناء البحث في المحتوي/التصدير
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/14/2020
ms.locfileid: "49676943"
---
# <a name="no-results-returned-during-content-searchexport"></a>لم يتم إرجاع اي نتائج اثناء البحث في المحتوي/التصدير

إذا كنت تواجه مشاكل في سيناريوهات eDiscovery التالية:

- لا ترجع ميزه البحث في المحتوي/التصدير اي بيانات أو بيانات غير متوقعه
- فشل البحث عن eDiscovery أو تصديره

قد يعود سبب ذلك إلى عوامل تصفيه أمان توافق معينه تم اعدادها بواسطة مسؤول معين ولم يتم الإبلاغ عن كل المسؤولين.

لحل هذه المشكلة ، تحقق مما إذا كانت هناك اي عوامل تصفيه أمان للتوافق قد تؤدي إلى حدوث هذه المشاكل:

1. الاتصال بمركز التوافق والأمان Powershell
2. قم بتشغيل الكوماندليتس التالية:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

للحصول علي معلومات اضافيه حول عوامل تصفيه أمان التوافق ، راجع [تصفيه الأذونات للبحث في المحتوي](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
