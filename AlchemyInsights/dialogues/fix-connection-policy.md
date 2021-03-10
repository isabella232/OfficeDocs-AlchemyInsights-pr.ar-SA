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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/09/2021
ms.locfileid: "50692512"
---
# <a name="fix-connection-policy"></a>إصلاح نهج الاتصال

تم وضع علامة آمن على البريد الإلكتروني وتسليمه إلى علبة الوارد الخاصة للمستخدم لأنه تم وضع علامة آمن على عنوان IP المرسل في نهج تصفية الاتصال. لمراجعة النهج، يمكنك القيام بما يلي:

1. انتقل إلى مركز التوافق & الأمان في [Office 365،](https://go.microsoft.com/fwlink/p/?linkid=2077143)ثم انتقل إلى نهج إدارة المخاطر   >    >  [لمكافحة البريد العشوائي.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. على علامة **التبويب "مخصص"،** حدد نهج **تصفية الاتصال،** ثم حدد **"تحرير النهج".**
3. راجع قائمة **السماح ب IP.** معرفة ما **إذا كانت القائمة الآمنة** تم تمكينها.

    > [!NOTE]
    > تشترك Microsoft في مصادر جهة خارجية للمرسلين الموثوق بهم. إذا **تم تمكين "القائمة** الآمنة"، لا يتم وضع علامة عن طريق الخطأ على هؤلاء المرسلين الموثوق بهم على أنها بريد عشوائي. من المستحسن تحديد هذا الخيار، لأنه سيقلل عدد الإيجابيات الخاطئة (البريد الجيد المصنف كبريد عشوائي) التي تتلقاها.
