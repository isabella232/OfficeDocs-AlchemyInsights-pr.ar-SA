---
title: استخدام Microsoft Intune أساسيات الأمان لتكوين أجهزة Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793530"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>استخدام Microsoft Intune أساسيات الأمان لتكوين أجهزة Windows 10

تساعد خطوط أمان Intune الأساسية على حماية المستخدمين والأجهزة. إن خطوط الأمان الأساسية Windows الإعدادات التي تم تكوينها مسبقا وتستخدم لتطبيق مجموعة معروفة من الإعدادات والقيم الافتراضية الموصى بها من قبل فرق الأمان ذات الصلة. من خلال إنشاء ملف تعريف أساسي أمان في Intune، يمكنك إنشاء قالب يتكون من ملفات تعريف تكوين أجهزة متعددة.

عند نشر خطوط الأمان الأساسية لمجموعات من المستخدمين أو الأجهزة، يتم تطبيق الإعدادات على الأجهزة التي يتم تشغيلها على Windows 10 أو لاحقا. على سبيل المثال، يقوم أساسا أمان إدارة أجهزة Microsoft المحمولة (MDM) تلقائيا بتمكين BitLocker لمحركات الأقراص القابلة للإزالة، ويتطلب كلمة المرور لإلغاء تأمين جهاز، ويعطل المصادقة الأساسية. عندما لا تعمل قيمة افتراضية مع بيئتك، يمكنك تخصيص الأساس لتطبيق الإعدادات التي تحتاج إليها.

تساعد خطوط الأمان الأساسية أيضا على إنشاء سير عمل آمن من النهاية إلى النهاية في Microsoft 365. يتضمن أساس الأمان أفضل الممارسات والتوصيات المتعلقة ب الإعدادات التي تؤثر على الأمان. يقوم Intune بالشركاء Windows فريق الأمان الذي ينشئ خطوط أساسية لنهج المجموعة، لذا تستند هذه التوصيات إلى إرشادات قوية وتجربة واسعة النطاق.

إذا كنت جديدا في Intune وغير متأكد من مكان البدء، فإن خطوط الأمان الأساسية تساعدك على إنشاء ملف تعريف آمن ونشره بسرعة. إذا كنت تستخدم حاليا نهج مجموعة، فإن عملية إجراء عملية إعادة التهجر إلى Intune لأغراض إدارية تكون أكثر سهولة مع خطوط الأمان الأساسية لأنها مضمنة في Intune وهي تتضمن قدرات الإدارة المتطورة.

لمعرفة المزيد، راجع Windows [أساسيات](/windows/security/threat-protection/windows-security-baselines) الأمان وإدارة [أجهزة المحمول](/windows/client-management/mdm/).

