---
title: إصلاح نهج الاتصال
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
ms.openlocfilehash: 7eae77358b0305582f53c411a092e3d2f1dbe17fd58ceac1ac00d5c07b3dd202
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988067"
---
# <a name="fix-connection-policy"></a>إصلاح نهج الاتصال

تم وضع علامة آمن على البريد الإلكتروني وتسليمه إلى علبة الوارد الخاصة به لأن عنوان IP المرسل تم وضع علامة آمن عليه في نهج عامل تصفية الاتصال. لمراجعة النهج، يمكنك القيام بما يلي:

1. انتقل إلى مركز Office 365 [الأمان &](https://go.microsoft.com/fwlink/p/?linkid=2077143)، ثم انتقل **إلى** نهج إدارة المخاطر لمكافحة البريد  >    >  [العشوائي.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. على علامة **التبويب مخصص،** حدد نهج **تصفية الاتصال**، ثم حدد **تحرير النهج**.
3. راجع قائمة **السماح ب IP.** معرفة **ما خزينة تم** تمكين القائمة.

    > [!NOTE]
    > تشترك Microsoft في مصادر جهة خارجية للمرسلين الموثوق بهم. إذا **خزينة القائمة،** لا يتم وضع علامة على هؤلاء المرسلين الموثوق بهم عن طريق الخطأ كبريد عشوائي. نوصي بتحديد هذا الخيار، لأنه سيقلل عدد الإيجابيات الخاطئة (البريد الجيد المصنف كبريد عشوائي) الذي تتلقاه.
