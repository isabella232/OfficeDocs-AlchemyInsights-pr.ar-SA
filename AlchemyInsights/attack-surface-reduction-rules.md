---
title: قواعد الحد من سطح الهجوم
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676043"
---
# <a name="attack-surface-reduction-rules"></a>قواعد الحد من سطح الهجوم

يمكن أن يقلل استبعاد الملفات أو المجلدات بشدة من الحماية التي توفرها قواعد تقليل مساحة الهجوم. يسمح بتشغيل الملفات التي تم حظرها بواسطة قاعدة، ولا يتم تسجيل أي تقرير أو حدث. ينطبق الاستثناء على كل القواعد التي تسمح بالاستثناءات.

تستخدم استثناءات ASR بناء الجملة نفسه الذي تستخدمه برنامج الحماية من الفيروسات من Microsoft Defender استثناءات. للحصول على التفاصيل، راجع [تكوين الاستثناءات](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus)لمسح برنامج الحماية من الفيروسات من Microsoft Defender والتحقق من صحتها . لتجنب المشاكل، راجع [الأخطاء الشائعة لتجنبها عند تعريف الاستثناءات.](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)

لا تدعم كل قواعد ASR الاستثناءات. للتحقق من صحة ما إذا كانت القاعدة تدعم الاستثناءات، راجع الجدول قواعد تقليل مساحة [الهجوم](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).

## <a name="attack-surface-reduction-rules"></a>قواعد الحد من سطح الهجوم

يتضمن سطح هجوم مؤسستك كل الأماكن التي يمكن أن يعرض فيها مهاجم أجهزة المؤسسة أو شبكاتها للخطر. يعني تقليل سطح الهجوم حماية أجهزة المؤسسة وشبكة الاتصال، مما يترك للمهاجمين طرقا أقل لتنفيذ الهجمات. يمكن أن يساعدك تكوين قواعد تقليل مساحة الهجوم في Microsoft Defender ل Endpoint.

لمزيد من المعلومات، اطلع على:

- [تعيين قاعدة ASR GUID إلى الاسم](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- متطلبات قواعد ASR:
    - [Windows 10 Pro الإصدار 1709 أو الإصدارات الأحدث](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows 10 Enterprise الإصدار 1709 أو الإصدارات الأحدث](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows الخادم، الإصدار 1803 (قناة نصف سنوية) أو إصدار أحدث](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a>تحديد الاستثناء الصحيح الذي يجب تطبيقه

1. ابحث عن eventID 1121 أو 1122 في سجل Microsoft-Windows-Windows Defender/Operational.

1. قم بتقييم سيناريو الكتلة وسياقها وتأكد من أنه يجب إلغاء حظر هذا السيناريو.

1. اقرأ القيمة Path في تفاصيل الحدث، وهي القيمة التي تعرف الاستثناء.
    - اجعل الاستثناء صارما قدر الإمكان.
    - تطبيق أحرف بدل عند الحاجة (على سبيل المثال، استبدال متغير المستخدم).

1. طبق الاستثناء وفقا لاحتياجات النشر. للحصول على التفاصيل، راجع [تخصيص قواعد تقليل مساحة الهجوم](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).

## <a name="exclusion-is-not-honored"></a>لا يتم احترام الاستثناء

1. تحديد ما إذا كانت القاعدة تدعم الاستثناءات أم لا. للحصول على التفاصيل، راجع [قواعد تقليل مساحة الهجوم](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).

1. راجع الاستثناءات المطبقة وتحقق من بيانات الحدث بسبب الأخطاء المطبعية أو أحرف البدل التي تم تفسيرها بشكل خاطئ. لمزيد من المعلومات، راجع [أنواع الاستثناءات المعتمدة](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)

1. إذا كان تأثير القاعدة عال جدا، فراجع نقل القاعدة (للخلف) إلى وضع التدقيق لتنفيذ المزيد من التحقق من الصحة. للحصول على التفاصيل، راجع [اختبار كيفية عمل ميزات Microsoft Defender لنقطة النهاية في وضع التدقيق](/microsoft-365/security/defender-endpoint/audit-windows-defender).

1. تجميع بيانات الدعم لفتح حالة دعم باستخدام هذا الأمر:
    
   ** MDEClientAnalyzer.cmd -v**

    لمزيد من المعلومات، راجع المشاكل المتعلقة [بآلات التكوين في Microsoft Defender لنقاط النهاية](issues-with-onboarding-machines.md).
