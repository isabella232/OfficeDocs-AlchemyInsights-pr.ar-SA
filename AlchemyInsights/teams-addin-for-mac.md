---
title: Teams الإضافية ل Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: c9c4eb811c93f6d11ebf606ba4bd20cddc2901d6616700ebfe6ef597dd8dc006
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940662"
---
# <a name="teams-add-in-for-mac"></a>Teams الإضافية ل Mac

لا استكشاف الأخطاء وإصلاحها في Teams الإضافية لمستخدمي نظام التشغيل Mac، اتبع الخطوات التالية:

**الخطوة 1:** إذا كان لديك Exchange مختلط (2016 CU3 أو الإصدارات اللاحقة مطلوبة)، فاستخدم أداة Test-HMA.ps1 لتأكيد تكوين المصادقة الحديثة المختلطة بشكل صحيح. لمزيد من المعلومات، راجع التحقق من صحة إعداد المصادقة الحديثة المختلطة [Outlook لنظامي التشغيل iOS وAndroid](https://aka.ms/TestHMAEAS).  

**ملاحظة** استخدم تنسيق عنوان UPN (على سبيل [المثال، username@contoso.com)،](mailto:username@contoso.com)وليس domain\username. يمكنك القيام بذلك حتى للمستخدمين الذين لديهم Exchange Online بريد.

**الخطوة 2:** هل تريد من المستخدم الانتقال إلى **أدوات**  >  **الحسابات**... في Outlook for Mac، واعثر على الحساب وحدده. تأكد من أن اسم المستخدم المدرج بتنسيق UPN (على سبيل [المثال،](mailto:username@contoso.com)username@contoso.com).

**الخطوة 3:** تأكد من أن المستخدم مستخدم Microsoft Teams مرخص. يجب أن يستخدم المستخدم Office 365 for Mac، إصدار المنتج 16.24 أو إصدار أحدث.