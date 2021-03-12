---
title: إصلاح قواعد النقل
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743393"
---
# <a name="fix-transport-rules"></a>إصلاح قواعد النقل

أثرت قاعدة تدفق بريد مخصصة على هذه الرسالة. لمراجعة القاعدة بدقة، يمكنك القيام بما يلي:

1. في نتائج الإرسال، ضمن **معلومات إضافية،** لاحظ **GUID** أو **اسم النهج**.
2. تشغيل Exchange Management Shell. لمزيد من المعلومات، [راجع فتح Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
3. تشغيل هذا الأمر (باستخدام GUID من الإرسال): **Get-TransportRule -identity "GUID"** | fl * الوصف*
4. راجع الوصف لرؤية الشروط التي تم تكوينها التي أثرت على الرسالة.

لمعرفة المزيد، راجع [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
