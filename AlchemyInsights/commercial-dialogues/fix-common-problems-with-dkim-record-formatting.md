---
title: إصلاح المشاكل الشائعة في تنسيق سجل DKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: e55175e7613d220eaf956d3c7fd02213dcd5803d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323977"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>إصلاح المشاكل الشائعة في تنسيق سجل DKIM

ترتبط معظم مشاكل إعداد DKIM بسجلات DNS غير الصحيحة.

لإصلاح مشاكل إعداد DKIM، تحقق من تنسيق سجل DKIM CNAME **(وليس** سجل TXT) بشكل صحيح. لمزيد من المعلومات، راجع ما يجب فعله لإعداد [DKIM](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)يدويا في Office 365 .

إذا كنت بحاجة إلى مساعدة في سجلات DNS بشكل عام، فشاهد إنشاء سجلات [DNS لدى أي موفر استضافة DNS Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).

**ملاحظة:** بعد إنشاء سجلات DNS DNS ل DKIM أو تحديثها في خدمة استضافة DNS لمجالك، ستحتاج إلى الانتظار حتى يتم نشر سجلات DNS.
