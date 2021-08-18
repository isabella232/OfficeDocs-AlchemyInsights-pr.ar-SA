---
title: مشاكل في تثبيت Microsoft Defender على Mac أو Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: ae17caa4be7809b591be9f9c042186f67828aa3c36a3d17332806e4d92545dc6
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898595"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>مشاكل في تثبيت Microsoft Defender على Mac أو Linux

**Mac**

- تأكد من تلبية متطلبات النظام قبل تثبيت Microsoft Defender ATP for Mac. لمزيد من المعلومات، [راجع كيفية تثبيت Microsoft Defender ATP for Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).  
- راجع المعلومات في الملف: "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- تأكد من تلبية متطلبات النظام قبل تثبيت Microsoft Defender ATP لنظام التشغيل Linux. لمزيد من المعلومات، [راجع كيفية تثبيت MDATP ل Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements). 
- للتحقق من تشغيل خدمة MDATP، راجع [فشل التثبيت](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).  
    لا استكشاف الأخطاء وإصلاحها في حالة عدم تشغيل الخدمة، راجع خطوات استكشاف الأخطاء وإصلاحها إذا لم تكن خدمة [mdatp](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)قيد التشغيل.
- للحصول على خطوات للتحقق من تكوين العميل، الذي يتحقق من صحة المنتج، ول تشغيل اختبار الكشف على الملف النصي EICAR، راجع [تكوين العميل](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).  

    **ملاحظة** للحصول على قائمة أنظمة الملفات المعتمدة للنشاط عند الوصول، راجع [Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).