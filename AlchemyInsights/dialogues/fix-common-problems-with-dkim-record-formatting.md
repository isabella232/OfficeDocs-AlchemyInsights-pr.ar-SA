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
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523147"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>إصلاح المشاكل الشائعة في تنسيق سجل DKIM

ترتبط معظم مشاكل إعداد DKIM بسجلات DNS غير صحيحة.

لإصلاح مشاكل إعداد DKIM، تحقق من تنسيق سجل DKIM CNAME **(وليس** سجل TXT) بشكل صحيح. لمزيد من المعلومات، راجع ما يجب فعله لإعداد [DKIM يدويا في Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)

إذا احتجت إلى مساعدة في سجلات DNS بشكل عام، فشاهد "إنشاء سجلات DNS" على أي موفر [استضافة DNS ل Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

> [!NOTE]
> بعد إنشاء سجلات DNS ل DKIM أو تحديثها في خدمة استضافة DNS لمجالك، ستحتاج إلى الانتظار حتى يتم نشر سجلات DNS.
