---
title: مراقبة الوصول المشروط إلى Intune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/03/2021
ms.locfileid: "50426992"
---
# <a name="monitor-intune-conditional-access"></a>مراقبة الوصول المشروط إلى Intune

سيتلقى المستخدمون المستهدفون الذين لديهم وصول شرطي بريدا إلكترونيا إعلاما إذا لم يلبيوا متطلبات الوصول إلى مؤسستك. لحل هذه المشكلة، نوصي باستخدام حل واحد أو أكثر من الحلول التالية:

1. إذا كان من المفترض أن يتم تسجيل الجهاز، فنصح المستخدمين بأن يقوموا الانتقال إلى تطبيق Company Portal وتحقق من ظهوره في Company Portal. وإذا لم يحدث ذلك، فيجب على المستخدم تسجيل الجهاز.
1. في مدخل Azure، انتقل إلى **توافق جهاز Intune.**  >   
1. لعرض تقرير توافق الجهاز للتحقق من وضع علامة على جهاز المستخدم كمتوافق، ضمن "جهاز العرض"، انقر فوق **توافق الجهاز.**
1. في مدخل Azure، انتقل إلى **توافق جهاز Intune.**  >   ضمن **"إدارة"، انقر** فوق **"سياسات".** في قائمة سياسات التوافق، تحقق من تعيين ملف تعريف إلى جهاز المستخدم. إذا لم يتم تعيين ملف تعريف، لن يتمكن Intune من تأكيد حالة توافق الجهاز.
1. تحرير تعيين الوصول المشروط للمستخدم.
1. في مدخل Azure، انتقل إلى نهج الوصول المشروط في **Intune،** وحدد نهج من القائمة، وانقر فوق المستخدمين  >    >   **والمجموعات.**
1. لاستهداف نهج معين لأحد الأشخاص، أضفه إلى القائمة **"تضمين".** للتأكد من حذف شخص من النهج، أضفه إلى القائمة **"استبعاد".**

**ارتباطات مفيدة:**

- [نظرة عامة حول توافق الجهاز](https://docs.microsoft.com/intune/device-compliance-get-started)
- [استكشاف الأخطاء الم CA وإصلاحها](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [نهج استكشاف الأخطاء وإصلاحها](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [مراقبة توافق أجهزة Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> هذه الخطوات مفيدة فقط في استكشاف الأخطاء في ميزة الوصول المشروط ل Azure Active Directory وإصلاحها. من الممكن أيضا فحص جهاز يمنع الوصول إلى البريد الإلكتروني الخاص به باستخدام نهج Exchange. يمكن العثور على مزيد من المعلومات حول إدارة أجهزة Exchange [**هنا.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))
