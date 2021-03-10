---
title: استخدام خطوط أمان Microsoft Intune لتكوين أجهزة Windows 10
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50692650"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a>استخدام خطوط أمان Microsoft Intune لتكوين أجهزة Windows 10

تساعد خطوط أمان Intune الأساسية على حماية المستخدمين والأجهزة. إن خطوط الأمان الأساسية هي مجموعات إعدادات Windows التي تم تكوينها مسبقا وتستخدم لتطبيق مجموعة معروفة من الإعدادات والقيم الافتراضية الموصى بها من قبل فرق الأمان ذات الصلة. من خلال إنشاء ملف تعريف أساسي أمان في Intune، يمكنك إنشاء قالب يتكون من ملفات تعريف تكوين جهاز متعددة.

عند نشر خطوط الأمان الأساسية لمجموعات من المستخدمين أو الأجهزة، يتم تطبيق الإعدادات على الأجهزة التي يتم تشغيلها على Windows 10 أو الإصدارات الأحدث. على سبيل المثال، يقوم أساس أمان إدارة أجهزة المحمول (MDM) من Microsoft تلقائيا (1) بتمكين BitLocker لمحركات الأقراص القابلة للإزالة، و(2) يتطلب كلمة المرور لإلغاء تأمين جهاز، و(3) تعطيل المصادقة الأساسية. عندما لا تعمل قيمة افتراضية مع بيئتك، يمكنك تخصيص الأساس لتطبيق الإعدادات التي تحتاجها.

تساعد خطوط الأمان الأساسية أيضا على إنشاء سير عمل آمن بشكل منته في Microsoft 365. فيما يلي بعض فوائد هذه الوظيفة:
- يتضمن أساس الأمان أفضل الممارسات والتوصيات المتعلقة ب الإعدادات التي تؤثر على الأمان. نظرا لأن Intune يعمل مع فريق أمان Windows الذي يقوم بإنشاء خطوط أساسية لنهج المجموعة، فإن هذه التوصيات تستند إلى إرشادات قوية وتجربة واسعة.
- إذا لم يكن Intune جديدا بالنسبة لك وغير متأكد من المكان الذي تريد البدء منه، فإن خطوط الأمان الأساسية ستساعدك على إنشاء ملف تعريف آمن ونشره بسرعة.
- إذا كنت تستخدم حاليا نهج مجموعة، فإن عملية التهجر إلى Intune لأغراض الإدارة تكون أكثر سهولة مع خطوط الأمان الأساسية، لأن خطوط الأمان الأساسية هذه مضمنة في Intune وتتضمن قدرات الإدارة المتطورة.

لمزيد من المعلومات، راجع خطوط [أمان Windows وإدارة](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) أجهزة [المحمول.](https://docs.microsoft.com/windows/client-management/mdm/)