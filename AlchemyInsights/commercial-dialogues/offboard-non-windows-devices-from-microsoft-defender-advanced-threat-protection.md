---
title: إيقاف تشغيل الأجهزة غير التي تعمل بنظام Windows من Microsoft Defender Advanced Threat Protection (ATP)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743038"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a>إيقاف تشغيل الأجهزة غير التي تعمل بنظام Windows من Microsoft Defender Advanced Threat Protection (ATP)

إليك كيفية تنفيذ ذلك:

1. اتبع وثائق جهة خارجية لقطع اتصال حل جهة خارجية من Microsoft Defender ATP.
2. من مستأجر Azure Active Directory، قم بإزالة الأذونات الخاصة بالحل الخاص ب جهة خارجية:

    1. سجل الدخول إلى [مدخل Azure](https://go.microsoft.com/fwlink/?linkid=2125612).
    1. حدد **كافة الخدمات**  >  **Azure Active Directory** Enterprise  >  **Applications**.
    1. حدد التطبيق الذي تريد إيقاف تشغيله.
    1. حدد **حذف**.

لمعرفة المزيد، راجع [إيقاف تشغيل الأجهزة غير التي تعمل بنظام التشغيل Windows](https://go.microsoft.com/fwlink/?linkid=2143630).
