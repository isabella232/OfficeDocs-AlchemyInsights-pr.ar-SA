---
title: Device Writeback
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8279"
ms.openlocfilehash: c069d0b4588e53250d6cc1f3a66c744ea5c12ae4
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320073"
---
# <a name="device-writeback"></a>Device Writeback

يتم استخدام Device Writeback في السيناريوهات التالية:

- تمكين [Windows Hello for Business باستخدام نشر الثقة في الشهادات المختلطة](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)
- تمكين الوصول الشرطي استنادا إلى الأجهزة إلى تطبيقات ADFS المحمية (2012 R2 أو أعلى) (ثقة الأطراف المعتمدة)

    **ملاحظة:** الاشتراك في Azure AD Premium مطلوب لكتابه الجهاز.

يوفر ذلك المزيد من الأمان وضمانة منح حق الوصول إلى التطبيقات للأجهزة الموثوق بها فقط. لمزيد من المعلومات حول الوصول الشرطي، [راجع](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) إدارة المخاطر باستخدام الوصول الشرطي وإعداد الوصول الشرطي في الموقع باستخدام تسجيل جهاز [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview).

لمزيد من المعلومات حول تمكين "إعادة كتابة الجهاز" للأجهزة، راجع [تمكين "إعادة كتابة الجهاز".](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback)
