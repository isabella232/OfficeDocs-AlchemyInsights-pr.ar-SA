---
title: علبة بريد الأرشيف ممتلئة تقريبا
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
ms.openlocfilehash: 085d9b211d5a8e9a0e1eb12af14d87a4e59c844a3afa012095dfd60db316ad14
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046739"
---
# <a name="your-archive-mailbox-is-almost-full"></a>علبة بريد الأرشيف ممتلئة تقريبا

إذا تلقى المستخدم التحذير؛ **إن علبة بريد الأرشيف ممتلئة تقريبا،** أو تحتاج إلى زيادة حجم علبة بريد الأرشيف، فيما يلي بعض التلميحات:

1. إذا تم تعيين ترخيص Exchange Online 1 للمستخدم، فترقية إلى Exchange Online **الخطة 2 لزيادة** الحجم من 50 غيغابايت إلى 100 غيغابايت.
1. إذا تم تعيين أي من المستخدمين بالفعل لأي من ما يلي: **Exchange Online الخطة 2** أو خطة Exchange Online 1 مع وظيفة أرشفة Exchange Online الإضافية، فاستخدم الخطوات أدناه لتمكين أرشفة التوسع التلقائي:.
 
    1. [الاتصال Exchange Online Powershell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)
    2. تشغيل الأمر التالي للمستخدم:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. تشغيل الأمر التالي لتأكيد تمكينه للمستخدم:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

لمزيد من المعلومات، راجع:

- [تمكين الأرشفة غير المحدودة - تعليمات المسؤول - Microsoft 365 التوافق | Microsoft Docs](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online حدود الخدمة - أوصاف | Microsoft Docs](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [الترقية إلى خطة عمل | Microsoft Docs](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

