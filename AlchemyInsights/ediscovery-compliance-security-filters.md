---
title: لم يتم إرجاع أي نتائج أثناء البحث/التصدير في المحتوى
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
ms.openlocfilehash: 5c04364f98dccbcad0f011df866f137d79c166ad3839b408d6be447d50a87ac3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101253"
---
# <a name="no-results-returned-during-content-searchexport"></a>لم يتم إرجاع أي نتائج أثناء البحث/التصدير في المحتوى

إذا كنت تواجه مشاكل في سيناريوهات eDiscovery التالية:

- لا يرجع البحث في المحتوى/التصدير أي بيانات أو بيانات غير متوقعة
- فشل البحث أو التصدير في eDiscovery

قد يعود سبب ذلك إلى بعض عوامل تصفية أمان التوافق التي تم إعدادها من قبل مسؤول معين ولم يتم إبلاغ جميع المسؤولين بها.

لحل هذه المشكلة، تحقق مما إذا كانت هناك أي عوامل تصفية أمان التوافق قد تتسبب في حدوث هذه المشاكل:

1. الاتصال إلى مركز الأمان والتوافق في Powershell
2. تشغيل الأوامر التالية:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

للحصول على معلومات إضافية حول عوامل تصفية أمان التوافق، راجع تصفية [الأذونات للبحث في المحتوى](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
