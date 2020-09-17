---
title: 932 ترقيه AADConnect
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
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806026"
---
# <a name="upgrade-azure-ad-connect"></a>ترقيه Azure AD Connect

بشكل افتراضي ، يتم تمكين الترقية التلقائية ل Azure AD Connect ، مما يساعد علي التاكد من تشغيل الإصدار الأخير. للتحقق من إعدادات الترقية التلقائية ، استخدم الأمر **أدسينكاوتوبجرادي** Cmdlet في Azure AD PowerShell. سيقوم أمر cmdlet بإرجاع أحدي القيم التالية:

- **ممكن**: تم تمكين الترقية التلقائية.

- **معطل**: تم تعطيل الترقية التلقائية.

- **معلق**: لم يعد النظام مؤهلا لتلقي الترقيات التلقائية. لا يمكنك تكوين هذه القيمة ؛ تم تعيينه بواسطة النظام.

لمزيد من المعلومات ، راجع [الترقية التلقائية](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

لتنزيل الإصدار الأخير من Azure AD Connect ، انتقل إلى [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
