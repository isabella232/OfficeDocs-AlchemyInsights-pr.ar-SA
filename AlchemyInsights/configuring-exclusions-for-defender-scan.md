---
title: تكوين الاستثناءات Microsoft Defender ATP المسح الضوئي
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
- "6027"
- "9001464"
ms.openlocfilehash: 5eb18f4133aca93c1506f4975c8d0567bede8d57
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543672"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a>تكوين الاستثناءات Microsoft Defender ATP المسح الضوئي

بشكل عام، يمكنك استثناء بعض ملحقات الملفات ومواقع المجلدات من Microsoft Defender ATP المسح الضوئي. يمكنك أيضا تكوين الاستثناءات للملفات التي يتم فتحها بواسطة عمليات معينة. لمزيد من المعلومات، [](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) راجع تكوين الاستثناءات والتحقق من صحتها استنادا إلى ملحق الملف وموقع المجلد وتكوين الاستثناءات للملفات التي يتم [فتحها بواسطة العمليات](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .

لتكوين استثناءات Windows **Server 2016 و2019،** راجع تكوين برنامج الحماية من الفيروسات من Microsoft Defender الاستثناءات على [Windows Server.](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)

**Mac**

للحصول على تفاصيل حول أنواع الاستثناءات المعتمدة وتكوين قائمة [](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) استثناءات ل Mac، راجع أنواع الاستثناءات المعتمدة وكيفية تكوين [قائمة الاستثناءات](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).

**ملاحظة** يمكنك أيضا التحقق من صحة قوائم الاستثناءات باستخدام ملف اختبار EICAR. لمزيد من المعلومات، راجع [التحقق من صحة قوائم الاستثناءات باستخدام ملف اختبار EICAR](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file). 

**Linux**

للحصول على تفاصيل حول أنواع الاستثناءات المعتمدة وتكوين قائمة [](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) استثناءات ل Linux، راجع أنواع الاستثناءات المعتمدة وتكوين الاستثناءات والتحقق [من صحتها Microsoft Defender ATP ل Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).

**ملاحظة** يمكنك أيضا التحقق من صحة قوائم الاستثناءات باستخدام ملف اختبار EICAR. لمزيد من المعلومات، راجع [التحقق من صحة قوائم الاستثناءات باستخدام ملف اختبار EICAR](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file). 