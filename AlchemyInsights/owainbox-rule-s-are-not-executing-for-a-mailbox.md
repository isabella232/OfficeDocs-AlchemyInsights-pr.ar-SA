---
title: 1332 OWA-قواعد علبة الوارد لا تنفذ لعلبة بريد
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 7d1848830847fc6722da20e09a4875f49bf02bd3
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/28/2019
ms.locfileid: "35360904"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>قاعدة الوارد لا يعمل كما هو متوقع

تحقق من الإعدادات التالية:

- يمكن إعادة توجيه رسالة، التي تم إعادة توجيهها أو الرد عليها تلقائياً استناداً إلى قواعد علبة الوارد مرة واحدة فقط. إضافة قاعدة إعادة توجيه (قاعدة علبة الوارد أو قاعدة تدفق البريد، تعرف أيضا باسم قاعدة نقل) كحد أقصى عشرة المستلمين إعادة التوجيه إلى رسالة. لمزيد من المعلومات، راجع [حدود قواعد دفتر اليومية، والنقل، وعلبة الوارد](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- لا تعمل قواعد علبة الوارد على علبة البريد اليومية بديلة. لمزيد من المعلومات حول البديل اليومية علبة البريد، راجع [علبة البريد اليومية بديلة](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

لحل هذه المشكلات، راجع [2829319 كيلو بايت](https://support.microsoft.com/kb/2829319).

إذا لم تقم بتطبيق الإعداد السابقة، تشغيل تقرير التشخيص قاعدة الوارد قبل أن يمكنك تصعيد المشكلة إلى "دعم microsoft":

1. فتح علبة البريد في Outlook على الويب، وانقر فوق **إعدادات** \> **خيارات** \> **تنظيم البريد الإلكتروني** \> **قواعد علبة الوارد**.

2. في أسفل الصفحة، انقر فوق **حالة القواعد لا تعمل انقر هنا لإنشاء تقرير تشخيص**.
