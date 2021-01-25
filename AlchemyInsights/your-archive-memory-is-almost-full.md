---
title: علبه بريد الأرشيف ممتلئة تقريبا
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974149"
---
# <a name="your-archive-mailbox-is-almost-full"></a>علبه بريد الأرشيف ممتلئة تقريبا

إذا تلقي المستخدم التحذير ؛ **ان علبه بريد الأرشيف الخاصة بك ممتلئة تقريبا**، أو انك تحتاج إلى زيادة حجم علبه بريد الأرشيف ، اليك بعض التلميحات:

1. إذا تم تعيين Exchange Online للخطة 1 ، فقم بالترقية إلى ترخيص **Exchange online الخطة 2** لزيادة الحجم من 50 غيغابايت إلى 100 غيغابايت.
1. إذا كان المستخدم قد قام بالفعل بتعيين اي من الخيارين التاليين: **Exchange online الخطة 2** أو exchange Online الخطة 1 مع وظيفة اضافيه للارشفه في Exchange online ، استخدم الخطوات التالية لتمكين أرشفه التوسيع التلقائي:.
 
    1. [الاتصال ب Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. قم بتشغيل الكوماندليت التالية للمستخدم:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. قم بتشغيل الكوماندليت التالية لتاكيد تمكينها للمستخدم:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

لمزيد من المعلومات ، راجع:

- [ تمكين الارشفه غير المحدودة-تعليمات المسؤول-توافق Microsoft 365 | مستندات Microsoft](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [حدود Exchange Online-أوصاف الخدمة | مستندات Microsoft](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [الترقية إلى خطه اعمال مختلفه | مستندات Microsoft](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

