---
title: خطأ ترخيص DLP لنقطة النهاية
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200001"
- "7176"
ms.openlocfilehash: 1e242abe18717e5ef64d6f067ab3ec6fa8833cb672dd21c85e577ce640240ba0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090112"
---
# <a name="endpoint-dlp-licensing-error"></a>خطأ ترخيص DLP لنقطة النهاية

عند محاولة إعداد نقطة نهاية DLP، إذا تلقيت رسالة الخطأ التالية:

`Your organization is missing the licenses required to manage these devices`.

تأكد من أن لديك أحد الاشتراكات أو الوظائف الإضافية التالية:

- Microsoft 365 E5
- Microsoft 365 A5 (EDU)
- Microsoft 365 E5 التوافق
- Microsoft 365 A5 التوافق
- Microsoft 365 E5 حماية المعلومات والحوكمة
- Microsoft 365 A5 حماية المعلومات والحوكمة

> [!NOTE]
> لن يعمل هذا الأمر مع مجموعات التراخيص مثل: Win E5 + O365 E5 + EMS E5. يجب أن يكون لديك ترخيص M365 E5 فقط لإعداد هذه الميزة.

لمزيد من معلومات ترخيص DLP لنقطة النهاية، راجع [ترخيص نقطة النهاية DLP.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
