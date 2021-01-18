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
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/15/2021
ms.locfileid: "49884775"
---
# <a name="configure-ldap"></a>تكوين LDAP

لتكوين LDAP ، نفذ الإجراءات التالية:

1. تحقق من صحة المجال علي [مدخل Azure](https://aka.ms/aadds-health).
1. تاكد من توفر اشتراك Azure AD صالح ومن تمكين خدمات مجال Azure AD.
1. يجب الحصول علي الشهادة المطلوبة لتمكين LDAP الامنه من مرجع مصدق عام موثوق به أو تكون شهادة موقعه ذاتيا.
1. تاكد من ان الشهادة تتبع [الإرشادات](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)المطلوبة.

**شهادة غير صالحه**
1. لتجديد شهادة ، اتبع الخطوات التالية لإنشاء شهادة جديده وريوبلواد: [تكوين LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. لحل المشكلة المعروفة باستخدام تنبيات LDAP الامنه في خدمات مجالات Azure Active directory ، راجع [حل تنبيات ldap](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
