---
title: لا تعمل المؤشرات باستخدام مستعرض Edge
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
- "11230"
- "9005470"
ms.openlocfilehash: ff7a2ee4c97c579422c7679c461f6fb288a9235ff9056be1c56e80b1d6379723
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/11/2021
ms.locfileid: "57887427"
---
# <a name="indicators-dont-work-using-edge-browser"></a>لا تعمل المؤشرات باستخدام مستعرض Edge

بعد إنشاء مؤشر، لن يتم احترامه بواسطة Edge (الشاشة الذكية). لمزيد من المعلومات، راجع [إنشاء مؤشرات ل IPs وURLs/domains](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain).

## <a name="step-1-ensure-the-following"></a>الخطوة 1: التأكد من ما يلي

- تحقق من صحة المؤشر (لا توجد أخطاء كتابية في IP/URL، الإجراء الصحيح، مجموعات RBAC الصحيحة).
- انتظر ساعتين كحد أدنى بعد إنشاء المؤشر لكي تأخذ في الاعتبار أي زمن قد يكون ممكنا.
- تأكد من أن النظام (الأنظمة) تم تشغيلها في Microsoft Defender لنقطة النهاية.
- تحقق من أن النظام (الأنظمة) يمكنه التواصل مع السحابة.
- تحقق من تمكين الشاشة الذكية والوصول إليها من خلال الذهاب إلى [موقع الاختبار](https://demo.smartscreen.msft.net).

## <a name="step-2-troubleshoot-the-potential-issue"></a>الخطوة 2: استكشاف المشكلة المحتملة وإصلاحها

- تأكد من أن العميل يلبي المتطلبات. للحصول على التفاصيل، راجع [إنشاء مؤشرات ل IPs وURLs/domains](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain).
- تأكد من تشغيل الإصدار الأخير من مستعرض Edge. لمعرفة الإصدار الأخير، راجع معرفة أي إصدار من Microsoft Edge [لديك](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).
- أعد تشغيل مستعرض Edge.
- انتقل إلى الموقع الذي قمت بإعداد مؤشر له. إذا لم يظهر الموقع كما هو متوقع، فتابع إلى الخطوة 3. 

## <a name="step-3-collect-data"></a>الخطوة 3: تجميع البيانات

- تجميع **بيانات MDEClientAnalyzer** التشخيصية. للحصول على الإرشادات، راجع المشاكل المتعلقة [بآلات التكوين في Microsoft Defender لنقطة النهاية](issues-with-onboarding-machines.md).
- إذا كنت مرتاحا لتثبيت تتبع Fiddler وجمعه، فشاهد [Telerik Fiddler](http://www.telerik.com/fiddler).
- إذا كنت تفضل الحصول على إرشادات من دعم Microsoft، فحدد أيقونة الدعم أدناه لفتح حالة دعم.
