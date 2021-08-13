---
title: تمكين المستخدم من مزامنة حساب شخصي مع حساب العمل في Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9127"
- "9004429"
ms.openlocfilehash: da435b37b689e97ca51ce5cf94eb7e7d71eb972060526989239310fac1460628
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813388"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>تمكين المستخدم من مزامنة حساب شخصي مع حساب العمل في Microsoft Edge

تأكد من أنك تفي بهذه المعايير:

- يتم تمكين تجوال حالة المؤسسة في مركز إدارة Azure Active Directory، الذي يتطلب اشتراكا في Azure Active Directory Premium أو Enterprise Mobility + Security (EMS). لمزيد من المعلومات، راجع [تمكين تجوال حالة المؤسسة في Azure Active Directory](/azure/active-directory/devices/enterprise-state-roaming-enable).
- يتم تطبيق معيار واحد أو كليهما:
    - تم تمكين خدمة Azure Information Protection للمستأجر. للحصول على التفاصيل، راجع [تنشيط حماية Azure Rights Management من مركز مسؤولي Microsoft 365](/azure/information-protection/activate-office365).
    - يتم تمكين ميزة تجوال حالة Azure Active Directory Enterprise (ESR) لأي مستخدم أو مستأجر. لمزيد من المعلومات، راجع [ما هو تجوال حالة المؤسسة؟](/azure/active-directory/devices/enterprise-state-roaming-overview).

إذا كان كل من AIP وESR معطلين، فإن رسالة خطأ تبلغ المستخدمين بأن المزامنة غير متوفرة للحسابات الخاصة بهم.
