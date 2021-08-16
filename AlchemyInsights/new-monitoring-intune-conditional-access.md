---
title: مراقبة الوصول الشرطي إلى Intune
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
ms.openlocfilehash: 7f30202ff0a5b9475393cf26c0506bd6bec24f3d378052f24ebf7f327cf84689
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54025489"
---
# <a name="monitor-intune-conditional-access"></a>مراقبة الوصول الشرطي إلى Intune

سيتلقى المستخدمون المستهدفون الذين لديهم حق وصول شرطي رسالة بريد إلكتروني إعلام إذا لم يلبيوا متطلبات الوصول الخاصة بالم مؤسستك. لحل هذه المشكلة، نوصي بحل واحد أو أكثر من الحلول التالية:

1. إذا كان من المفترض أن يكون الجهاز مسجلا، فنصح المستخدم الانتقال إلى تطبيق Company Portal وتحقق من ظهوره في Company Portal. وإذا لم يحدث ذلك، فيجب على المستخدم تسجيل الجهاز.
1. في مدخل Azure، انتقل إلى **توافق جهاز Intune**  >  . 
1. لعرض تقرير توافق جهازك للتحقق من وضع علامة على جهاز المستخدم كمتوافق، ضمن جهاز **العرض،** انقر فوق **توافق الجهاز.**
1. في مدخل Azure، انتقل إلى **توافق جهاز Intune**  >  . ضمن **إدارة، انقر** فوق **سياسات**. في قائمة سياسات التوافق، تحقق من تعيين ملف تعريف إلى جهاز المستخدم. إذا لم يتم تعيين ملف تعريف، لن يتمكن Intune من تأكيد حالة توافق الجهاز.
1. تحرير تعيين الوصول الشرطي للمستخدم.
1. في مدخل Azure، انتقل إلى نهج الوصول الشرطي **في Intune**، وحدد نهج من القائمة، وانقر  >    >  فوق **المستخدمون والمجموعات**.
1. لاستهداف نهج معين لشخص ما، قم بإضافته إلى **القائمة تضمين**. للتأكد من حذف شخص من النهج، قم بإضافته إلى القائمة **استبعاد**.

**ارتباطات مفيدة:**

- [نظرة عامة حول توافق الجهاز](https://docs.microsoft.com/intune/device-compliance-get-started)
- [استكشاف الأخطاء الم CA وإصلاحها](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [نهج استكشاف الأخطاء وإصلاحها](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [مراقبة توافق أجهزة Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> هذه الخطوات مفيدة فقط في استكشاف الأخطاء وإصلاحها في ميزة Azure Active Directory الوصول الشرطي. من الممكن أيضا فحص جهاز يمنع الوصول إلى البريد الإلكتروني باستخدام Exchange المستخدم. يمكنك العثور على Exchange إضافية حول إدارة الأجهزة [**هنا.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))
