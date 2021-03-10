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
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/09/2021
ms.locfileid: "50692510"
---
# <a name="fix-transport-rules"></a>إصلاح قواعد النقل

أثرت قاعدة تدفق بريد مخصصة على هذه الرسالة. لمراجعة القاعدة بدقة، يمكنك القيام بما يلي:

1. في نتائج الإرسال، ضمن **المعلومات الإضافية،** لاحظ **GUID** أو **اسم النهج.**
2. تشغيل Exchange Management Shell. لمزيد من المعلومات، راجع [فتح Exchange Management Shell.](https://go.microsoft.com/fwlink/?linkid=2101432)
3. تشغيل هذا الأمر (باستخدام GUID من الإرسال):  **Get-TransportRule -identity "GUID" | fl * الوصف***
4. راجع الوصف لرؤية الشروط التي تم تكوينها التي أثرت على الرسالة.

لمعرفة المزيد، راجع [Get-TransportRule.](https://go.microsoft.com/fwlink/?linkid=2101523)
