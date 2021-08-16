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
ms.openlocfilehash: 78af4dc8cfe38586dcec8d01b72170b56d98fa27860489bf2ca9544f32210c37
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101937"
---
# <a name="device-writeback"></a>Device Writeback

يتم استخدام Device Writeback في السيناريوهات التالية:

- تمكين [Windows Hello for Business باستخدام نشر الثقة بالشهادات المختلطة](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)
- تمكين الوصول الشرطي استنادا إلى الأجهزة إلى تطبيقات ADFS المحمية (2012 R2 أو أعلى) (ثقة الأطراف المعتمدة)

    > [!NOTE]
    > الاشتراك في Azure AD Premium مطلوب لكتابه الجهاز.

يوفر ذلك المزيد من الأمان وضمانة منح حق الوصول إلى التطبيقات للأجهزة الموثوق بها فقط. لمزيد من المعلومات حول الوصول الشرطي، [راجع](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) إدارة المخاطر باستخدام الوصول الشرطي وإعداد الوصول الشرطي في الموقع باستخدام تسجيل جهاز [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview).

لمزيد من المعلومات حول تمكين "إعادة كتابة الجهاز" للأجهزة، راجع [تمكين "إعادة كتابة الجهاز".](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback)
