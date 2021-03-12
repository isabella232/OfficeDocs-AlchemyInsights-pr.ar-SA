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
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743407"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>إصلاح المشاكل الشائعة في تنسيق سجل DKIM

ترتبط معظم مشاكل إعداد DKIM بسجلات DNS غير الصحيحة.

لإصلاح مشاكل إعداد DKIM، تحقق من تنسيق سجل DKIM CNAME **(وليس** سجل TXT) بشكل صحيح. لمزيد من المعلومات، راجع ما يجب فعله لإعداد [DKIM يدويا في Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).

إذا كنت بحاجة إلى مساعدة في سجلات DNS بشكل عام، فشاهد إنشاء [سجلات DNS لدى أي موفر استضافة DNS ل Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).

> [!NOTE]
> بعد إنشاء سجلات DNS DKIM أو تحديثها في خدمة استضافة DNS لمجالك، ستحتاج إلى انتظار نشر سجلات DNS.
