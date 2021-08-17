---
title: 1332 OWA - لا يتم تنفيذ قاعدة (قواعد) علبة الوارد لعلبة بريد
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
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: b05ed9f0ee8c18b49b5338c53e67a79f1bf65464385dfa0ebd0639172a1b18f2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040889"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>لا تعمل قاعدة علبة الوارد كما هو متوقع

تحقق من الإعدادات التالية في Outlook على ويب:

- يمكن إعادة توجيه رسالة أو إعادة توجيهها أو ردها تلقائيا استنادا إلى قواعد علبة الوارد مرة واحدة فقط. يمكن لقاعدة إعادة التوجيه (قاعدة علبة الوارد أو قاعدة تدفق البريد، المعروفة أيضا باسم قاعدة النقل) إضافة عشرة مستلمين لإعادة التوجيه كحد أقصى إلى رسالة. لمزيد من المعلومات، راجع حدود قواعد دفتر [اليومية والنقل علبة الوارد](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- لا تعمل قواعد علبة الوارد على علبة البريد البديلة الخاصة بعمل اليومية. لمزيد من المعلومات حول علبة بريد دفتر اليومية البديلة، راجع [علبة بريد دفتر اليومية البديلة](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

لإصلاح هذه المشاكل، راجع [KB 2829319](https://support.microsoft.com/kb/2829319).

إذا لم تنطبق المشاكل السابقة، فقم بتشغيل التقرير التشخيصي لقاعدة علبة الوارد قبل تصعيد المشكلة إلى دعم Microsoft:

1. افتح علبة البريد في Outlook على ويب، وانقر فوق <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **الإعدادات**  >  **عرض كل Outlook الإعدادات**  >  **البريد**  >  **القواعد**.

2. في أسفل الصفحة، انقر فوق إذا كانت القواعد لا تعمل، انقر هنا **لإنشاء تقرير تشخيصي.**
