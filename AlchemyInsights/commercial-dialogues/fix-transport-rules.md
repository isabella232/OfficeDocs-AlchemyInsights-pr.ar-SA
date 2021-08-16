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
ms.openlocfilehash: d89283dec427ba3d4f55fc1f180efc13da16ae15c3d5a6c0c06a696faa6df7f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034741"
---
# <a name="fix-transport-rules"></a>إصلاح قواعد النقل

أثرت قاعدة تدفق بريد مخصصة على هذه الرسالة. لمراجعة القاعدة بدقة، يمكنك القيام بما يلي:

1. في نتائج الإرسال، ضمن **معلومات إضافية،** لاحظ **GUID** أو **اسم النهج**.
2. تشغيل Exchange Management Shell. لمزيد من المعلومات، راجع [فتح Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
3. تشغيل هذا الأمر (باستخدام GUID من الإرسال): **Get-TransportRule -identity "GUID"** | fl * الوصف*
4. راجع الوصف لرؤية الشروط التي تم تكوينها التي أثرت على الرسالة.

لمعرفة المزيد، راجع [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
