---
title: تعيين دور "سجل التدقيق" في مركز التوافق & أمان Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743118"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a>تعيين دور "سجل التدقيق" في مركز التوافق & أمان Office 365

للبحث في سجل تدقيق Office 365، يجب أن يتم تعيين دور "سجلات التدقيق ل **View-only"** أو دور "سجلات التدقيق" في Exchange Online.  يتم تعيين هذه الأدوار إلى مجموعات أدوار إدارة التوافق وإدارة المؤسسة بشكل افتراضي. يضاف تلقائيا المسؤولون العامون في Office 365 و Microsoft 365 كأعضاء في مجموعة دور إدارة المؤسسة.

لتمكين المستخدم من البحث بأقل مستوى من الامتيازات، أنشئ مجموعة دور مخصصة  في Exchange Online،  وأضف دور "سجلات التدقيق" ل "طريقة العرض فقط" أو دور "سجلات التدقيق"، ثم أضف المستخدم كعضو في مجموعة الدور الجديدة.

لمزيد من المعلومات، راجع [إدارة مجموعات الدور في Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) والبحث في سجل التدقيق في مركز & [التوافق.](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)