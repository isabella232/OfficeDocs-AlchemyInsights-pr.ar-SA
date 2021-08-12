---
title: مشاكل في استخدام وحدة تحكم مسؤول Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 9310e8685a922207be8d5672d7929e19313cbb57e0fa6d25de149106692e811f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53944118"
---
# <a name="problems-using-the-intune-admin-console"></a>مشاكل في استخدام وحدة تحكم مسؤول Intune

**"تم رفض الوصول" عند التنقل في مدخل مسؤول Intune.**

- إذا كنت عضوا في دور مخصص في Intune، فتأكد من تعيين ترخيص Intune أو Enterprise Mobility Suite (EMS) إلى حسابك.
- إذا كنت تستخدم "إدارة التكوين" لإدارة الأجهزة، فتحقق من أنك لست جزءا من مجموعة المستخدمين Intune ل MDM "إدارة التكوين".
- تحقق من أنه تم تعيين أذونات التحكم في الإدارة المناسبة المستندة إلى الدور (RBAC) في شفرة أدوار Intune.
- تحقق من أن المجموعة المستخدمة ليست قائمة توزيع. يدعم Intune في مدخل Azure فقط حسابات المستخدمين التي تنتمي إلى مجموعات أمان Azure Active Directory. راجع المجموعات في مدخل Azure > **Intune** Groups أو في مدخل Azure >  >   **Azure Active Directory**.

**لدى المستخدم عدد كبير جدا من الأذونات لدور Intune المعين**

ننصح المستخدمين الانتقال إلى **أدوار Intune**  >  **Intune** الأذونات  >    >  **تصدير** لمراجعة الأذونات الممنوحة.

**لقد أضفت مجموعة نطاق إلى دور، ولكن لا يزال المستخدمون في هذا الدور يرون مستخدمين آخرين أو أجهزة أخرى.**

لا تقوم مجموعات النطاقات بتصفية المستخدمين أو الأجهزة. مجموعات النطاقات:

- تحديد الأشخاص الذين يمكن للمستخدمين تعيين سياسات أو تطبيقات له.
- السماح لمستخدمين محددين فقط بتشغيل المهام البعيدة على الأجهزة.

لمزيد من المعلومات حول مجموعات النطاقات، راجع التحكم بالوصول المستند إلى الدور [(RBAC) مع Microsoft Intune.](https://docs.microsoft.com/intune/role-based-access-control)

**لقد أضفت مستخدما إلى دور Intune ولكن لا يزال لديه حق الوصول الكامل إلى وحدة تحكم مسؤول Intune.**

انتقل إلى Intune > **المستخدمين** في مدخل Azure وتحقق من عدم تعيين المستخدم لأي من الأدوار التالية في مدخل Azure:

- المسؤول العام
- مسؤول خدمة Intune
- SharePoint مسؤول

لمزيد من المعلومات، راجع التحكم بالوصول المستند إلى [الدور (RBAC) مع Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**مشاكل الوصول**

لمزيد من المعلومات، راجع لا يمكنك تسجيل الدخول إلى Office 365 [أو Azure أو Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).