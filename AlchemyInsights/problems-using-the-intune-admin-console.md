---
title: المشاكل المتعلقة باستخدام وحده تحكم مسؤول Intune
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
ms.openlocfilehash: 10b37b2ffda50dc77396039a9e0e443ad81aef72
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728274"
---
# <a name="problems-using-the-intune-admin-console"></a>المشاكل المتعلقة باستخدام وحده تحكم مسؤول Intune

**"تم رفض الوصول" عند التنقل في مدخل مسؤول Intune.**

- إذا كنت عضوا في دور Intune مخصص ، فتاكد من انه تم تعيين ترخيص المجموعة "الخاصة ب Intune" (EMS) لحسابك.
- إذا كنت تستخدم أداره التكوين لأداره الاجهزه ، فتحقق من انك لست جزءا من مجموعه مستخدمي Intune لأداره التكوين MDM.
- تاكد من انك قمت بتعيين أذونات التحكم المناسبة المستندة إلى الدور (RBAC) في ريش ادوار Intune.
- تاكد من ان المجموعة المستخدمة ليست قائمه توزيع. يعتمد Intune في مدخل Azure حسابات المستخدمين الذين ينتمون إلى مجموعات أمان Azure Active directory فقط. قم بمراجعه مجموعاتك في مجموعات azure portal > **Intune**  >  **Groups**، أو في azure portal > **Azure active**directory.

**يملك المستخدم العديد من الأذونات لدور Intune المعين**

قم باعلام المستخدم بالانتقال إلى ادوار **intune**  >  **intune**  >  **الخاصة بي**  >  **Export** لمراجعه الأذونات الممنوحة.

**لقد أضفت مجموعه نطاقات إلى أحد الأدوار ، ولكن ما زال بإمكان المستخدمين في هذا الدور رؤية المستخدمين أو الاجهزه الأخرى.**

لا تقوم مجموعات النطاقات بتصفية المستخدمين أو الاجهزه. مجموعات النطاقات:

- تحديد الأشخاص الذين يمكنهم تعيين النهج أو التطبيقات اليهم.
- السماح لمستخدمين محددين فقط بتشغيل المهام البعيدة علي الاجهزه.

للحصول علي مزيد من المعلومات حول مجموعات النطاقات ، راجع  [التحكم في الوصول القائم علي الدور (RBAC) باستخدام Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**لقد أضفت مستخدما إلى دور Intune ولكنه ما زال لديه حق الوصول الكامل إلى وحده تحكم مسؤول Intune.**

انتقل إلى Intune > **المستخدمين** في مدخل Azure وتحقق من عدم تعيين المستخدم إلى اي من الأدوار التالية في مدخل azure:

- المسؤول العام
- مسؤول خدمه Intune
- مسؤول SharePoint

للحصول علي مزيد من المعلومات ، راجع [التحكم في الوصول القائم علي الأدوار (RBAC) باستخدام Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**مشاكل في الوصول**

لمزيد من المعلومات ، راجع [لا يمكنك تسجيل الدخول إلى Office 365 أو Azure أو Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).