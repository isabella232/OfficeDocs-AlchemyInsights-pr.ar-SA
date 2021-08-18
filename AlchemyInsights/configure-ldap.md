---
title: تكوين LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: 3f1f9728cdcfbe5676e5afc45b2afe82836fed9c8907df3559ac7daec21194ed
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090399"
---
# <a name="configure-ldap"></a>تكوين LDAP

لتكوين LDAP، قم بما يلي:

1. تحقق من صحة مجالك على مدخل [Azure](https://aka.ms/aadds-health).
1. تأكد من توفر اشتراك Azure AD صالح وتمكين Azure AD Domain Services.
1. يجب الحصول على الشهادة المطلوبة لتمكين LDAP الآمن من مرجع ممصادقة عام موثوق به أو أن تكون شهادة موقعة ذاتيا.
1. تأكد من أن الشهادة تتبع [الإرشادات المطلوبة.](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)

**شهادة غير صالحة**
1. لتجديد شهادة، اتبع الخطوات لإنشاء شهادة جديدة ثم إعادة تحميل: [تكوين LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. لحل المشكلة المعروفة في تأمين تنبيهات LDAP في Azure Active directory Domain Services، راجع [حل تنبيهات LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
