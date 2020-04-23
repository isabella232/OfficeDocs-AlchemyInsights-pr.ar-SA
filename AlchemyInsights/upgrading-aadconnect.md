---
title: 932 ترقية AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766480"
---
# <a name="upgrade-azure-ad-connect"></a>ترقية اتصال Azure AD

بشكل افتراضي، يتم تمكين الترقية التلقائية لـ Azure AD Connect، مما يساعد على ضمان تشغيل أحدث إصدار. للتحقق من إعدادات الترقية التلقائية، استخدم **cmdlet Get-ADSyncAutoUpgrade** في Azure AD PowerShell. سيعود cmdlet إحدى القيم التالية:

- **ممكّن:** تم تمكين الترقية التلقائية.

- **معطل:** تم تعطيل الترقية التلقائية.

- **مع وقف التنفيذ:** لم يعد النظام مؤهلاً لتلقي ترقيات تلقائية. لا يمكنك تكوين هذه القيمة; تم تعيينها من قبل النظام.

لمزيد من المعلومات، راجع [الترقية التلقائية](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

لتحميل أحدث إصدار من Azure AD [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)Connect، انتقل إلى .
