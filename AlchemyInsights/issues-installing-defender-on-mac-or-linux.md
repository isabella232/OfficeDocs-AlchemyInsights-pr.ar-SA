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
ms.openlocfilehash: a8d5ad2246b9b83e1e0a4d5be4dd8bb41c16e734
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713254"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>مشاكل في تثبيت Microsoft Defender على Mac أو Linux

**Mac**

- تأكد من تلبية متطلبات النظام قبل تثبيت Microsoft Defender ATP for Mac. لمزيد من المعلومات، [راجع كيفية تثبيت Microsoft Defender ATP for Mac.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)  
- راجع المعلومات في الملف: "/Library/Logs/Microsoft/mdatp/install.log".

**Linux**

- تأكد من تلبية متطلبات النظام قبل تثبيت Microsoft Defender ATP ل Linux. لمزيد من المعلومات، [راجع كيفية تثبيت Microsoft Defender ATP ل Linux.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements) 
- للتحقق من تشغيل خدمة MDATP، راجع [فشل التثبيت.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)  
    استكشاف المشاكل وإصلاحها إذا لم تكن الخدمة قيد التشغيل، راجع خطوات استكشاف الأخطاء وإصلاحها إذا لم تكن خدمة [mdatp قيد التشغيل.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)
- للحصول على خطوات للتحقق من تكوين العميل، الذي يتحقق من صحة المنتج، وتشغيل اختبار الكشف على الملف النصي EICAR، راجع [تكوين العميل.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration)  

    **ملاحظة** للحصول على قائمة أنظمة الملفات المعتمدة لنشاط عند الوصول، راجع [Microsoft Defender ATP for Linux.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)