---
title: مشاكل في استخدام وحدة تحكم المسؤول Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/29/2020
ms.locfileid: "46554728"
---
# <a name="problems-using-the-intune-admin-console"></a>مشاكل في استخدام وحدة تحكم المسؤول Intune

**"تم رفض الوصول" عند التنقل في مدخل مسؤول Intune.**

- إذا كنت عضوًا في دور مخصص Intune، تأكد من تعيين ترخيص Intune أو مجموعة التنقل المؤسسي (EMS) إلى حسابك.
- إذا كنت تستخدم إدارة التكوين لإدارة الأجهزة، تحقق من أنك لست جزءًا من مجموعة المستخدمين Intune لـ إدارة التكوين MDM.
- تحقق من أنه تم تعيين الأذونات المناسبة للتحكم بالإدارة المستندة إلى الدور (RBAC) في النصل أدوار Intune.
- تحقق من أن المجموعة المستخدمة ليست قائمة توزيع. Intune في البوابة الإلكترونية أزور فقط يدعم حسابات المستخدمين التي تنتمي إلى مجموعات أمان Azure Active Directory. راجع المجموعات الخاصة بك في البوابة Azure > مجموعات **إينتوني**  >  **Groups**، أو في بوابة Azure > Azure **Active Directory**.

**المستخدم لديه الكثير من الأذونات لدور Intune المعينة**

تقديم المشورة للمستخدم للانتقال إلى **Intune**  >  **Intune الأدوار**بلدي  >  **أذونات**  >  **تصدير** لمراجعة الأذونات الممنوحة.

**لقد أضفت مجموعة نطاق إلى دور ما، ولكن لا يزال المستخدمون في هذا الدور يرون مستخدمين آخرين أو أجهزة أخرى.**

لا تقوم مجموعات النطاق بتصفية المستخدمين أو الأجهزة. مجموعات النطاق:

- تحديد الأشخاص الذين يمكن للمستخدمين تعيين نُهج أو تطبيقات لهم.
- السماح لمستخدمين معينين فقط بتشغيل المهام البعيدة على الأجهزة.

لمزيد من المعلومات حول مجموعات النطاق، راجع [التحكم بالوصول إلى الأدوار (RBAC) مع Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**أضفت مستخدمًا إلى دور Intune ولكن لا يزال لديهم حق الوصول الكامل إلى وحدة تحكم Intune admin.**

انتقل إلى إينتوني > **المستخدمين** في البوابة الإلكترونية أزور وتحقق من أن المستخدم لم يتم تعيين إلى أي من الأدوار التالية في المدخل Azure:

- مسؤول عمومي
- مسؤول خدمة Intune
- مسؤول SharePoint

لمزيد من المعلومات، راجع [التحكم في الوصول المستند إلى الدور (RBAC) مع Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**مشاكل الوصول**

لمزيد من المعلومات، راجع [لا يمكنك تسجيل الدخول إلى Office 365 أو Azure أو Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).