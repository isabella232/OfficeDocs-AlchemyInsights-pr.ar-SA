---
title: 932 ترقية AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9582f1f56e6730e35520b5d79bc245cd74bea0bf4db39b379a7cd133bafc16ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104799"
---
# <a name="upgrade-azure-ad-connect"></a>ترقية Azure AD الاتصال

بشكل افتراضي، يتم تمكين الترقية التلقائية ل Azure AD الاتصال، مما يساعد على ضمان تشغيل الإصدار الأخير. للتحقق من إعدادات الترقية التلقائية، استخدم **أمر cmdlet Get-ADSyncAutoUpgrade** في Azure AD PowerShell. سيرجع cmdlet إحدى القيم التالية:

- **تمكين**: يتم تمكين الترقية التلقائية.

- **معطل**: يتم تعطيل الترقية التلقائية.

- **معلق**: لم يعد النظام مؤهلا لتلقي الترقيات التلقائية. لا يمكنك تكوين هذه القيمة؛ يتم تعيينه بواسطة النظام.

لمزيد من المعلومات، راجع [الترقية التلقائية](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

لتنزيل أحدث إصدار من Azure AD الاتصال، انتقل إلى [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
