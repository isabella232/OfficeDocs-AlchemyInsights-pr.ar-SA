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
ms.openlocfilehash: f1a8dba19d220e1154549507801c813f56fe5cdd
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256659"
---
# <a name="device-writeback"></a>Device Writeback

يتم استخدام Device Writeback في السيناريوهات التالية:

- تمكين [Windows Hello for Business باستخدام نشر الثقة بالشهادات المختلطة](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)
- تمكين الوصول الشرطي استنادا إلى الأجهزة التي تم توفيرها للتطبيقات المحمية من ADFS (2012 R2 أو أعلى) (ثقة الطرف المعتمد)

    > [!NOTE]
    > الاشتراك في Azure AD Premium مطلوب لكتابه الجهاز.

ويوفر ذلك المزيد من الأمان وضمانة أن الوصول إلى التطبيقات يتم منحه للأجهزة الموثوق بها فقط. للحصول على مزيد من [](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) المعلومات حول "الوصول الشرطي"، راجع "إدارة المخاطر" باستخدام "الوصول المشروط" وإعداد "الوصول المشروط" في الموقع باستخدام تسجيل جهاز [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/devices/overview)

لمزيد من المعلومات حول تمكين "إعادة كتابة الجهاز" للأجهزة، راجع ["تمكين كتابة الجهاز".](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback)
