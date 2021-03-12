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
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a><span data-ttu-id="f3b8b-102">تعيين دور "سجل التدقيق" في مركز التوافق & أمان Office 365</span><span class="sxs-lookup"><span data-stu-id="f3b8b-102">Assign an Audit Log role in the Office 365 Security & Compliance Center</span></span>

<span data-ttu-id="f3b8b-103">للبحث في سجل تدقيق Office 365، يجب أن يتم تعيين دور "سجلات التدقيق ل **View-only"** أو دور "سجلات التدقيق" في Exchange Online. </span><span class="sxs-lookup"><span data-stu-id="f3b8b-103">To search the Office 365 audit log, an administrator must be assigned the **View-Only Audit Logs** role or the **Audit Logs** role in Exchange Online.</span></span> <span data-ttu-id="f3b8b-104">يتم تعيين هذه الأدوار إلى مجموعات أدوار إدارة التوافق وإدارة المؤسسة بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="f3b8b-104">These roles are assigned to the Compliance Management and Organization Management role groups by default.</span></span> <span data-ttu-id="f3b8b-105">يضاف تلقائيا المسؤولون العامون في Office 365 و Microsoft 365 كأعضاء في مجموعة دور إدارة المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="f3b8b-105">Global administrators in Office 365 and Microsoft 365 are automatically added as members of the Organization Management role group.</span></span>

<span data-ttu-id="f3b8b-106">لتمكين المستخدم من البحث بأقل مستوى من الامتيازات، أنشئ مجموعة دور مخصصة  في Exchange Online،  وأضف دور "سجلات التدقيق" ل "طريقة العرض فقط" أو دور "سجلات التدقيق"، ثم أضف المستخدم كعضو في مجموعة الدور الجديدة.</span><span class="sxs-lookup"><span data-stu-id="f3b8b-106">To enable a user to search with the minimum level of privileges, create a custom role group in Exchange Online, add the **View-Only Audit Logs** role or **Audit Logs** role, and then add the user as a member of the new role group.</span></span>

<span data-ttu-id="f3b8b-107">لمزيد من المعلومات، راجع [إدارة مجموعات الدور في Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) والبحث في سجل التدقيق في مركز & [التوافق.](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)</span><span class="sxs-lookup"><span data-stu-id="f3b8b-107">For more information, see [Manage role groups in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) and [Search the audit log in the Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>