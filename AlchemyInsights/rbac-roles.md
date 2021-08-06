---
title: 'أدوار RBAC '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 1faa9f69942d39b8d78c8f3e1316f93b52eeede6408dfabc89d0f7fe38b86fb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923112"
---
# <a name="rbac-rules"></a>قواعد RBAC

إذا حصلت على خطأ الإذن: 

- ليس لدى العميل الذي لديه هوية كائن تخويل لتنفيذ إجراء عبر النطاق **(التعليمات البرمجية: AuthorizationFailed)**: عندما تحاول إنشاء مورد، تحقق من تسجيل الدخول حاليا مع مستخدم تم تعيين دور له إذن الكتابة للمورد في النطاق المحدد. على سبيل المثال، لإدارة الأجهزة الظاهرية في [](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) مجموعة موارد، يجب أن يكون لديك دور المساهم الظاهري في الجهاز على مجموعة الموارد (أو النطاق الأصل). للحصول على قائمة بالأذونات لكل دور مضمن، راجع الأدوار المضمنة [في موارد Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- ليس لديك الإذن لإنشاء طلب دعم **:** عند محاولة إنشاء تذكرة دعم أو تحديثها، تحقق من أنك قمت حاليا تسجيل الدخول باستخدام مستخدم تم تعيين دور له إذن Microsoft.support/supportTickets/write، مثل "مساهم [طلب](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)الدعم".
- لا يمكن إنشاء المزيد من تعيينات الدور **(التعليمات البرمجية: RoleAssignmentLimitExceeded)**: عندما تحاول تعيين دور، حاول تقليل عدد تعيينات الدور من خلال تعيين أدوار للمجموعات بدلا من ذلك. يدعم Azure ما يصل إلى **2000** تعيين دور لكل اشتراك.

لمزيد من التفاصيل حول أدوار Azure RBAC، راجع [أدوار Azure RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
