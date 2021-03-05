---
title: تكوين خدمة مزامنة MIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "50480838"
---
# <a name="configure-mim-sync-service"></a>تكوين خدمة مزامنة MIM

إن خدمة مزامنة Microsoft Identity Manager (MIM) هي أحد مكونات MIM. إنها خدمة مركزية في الموقع المحلية تخزن المعلومات وتكاملها مع المؤسسات التي لديها العديد من الدلائل وقواعد البيانات المحلية. قد تتمكن من حل مشكلتك في "مزامنة MIM" إذا تم حل المشكلة في تحديث حديث ل MIM أو إذا كانت إحدى المشاكل الأخرى المذكورة في القسم أدناه.

**الخطوات المستحسنة**

1. تأكد من أنك تستخدم تحديثا حديثا لمزامنة MIM وتحقق من ملاحظات إصدار [مزامنة MIM](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) لتحديد ما إذا تم حل المشكلة في تحديث.
2. إذا كانت المشكلة في موصل GENERIC LDAP أو SQL العام أو Lotus Domino أو Web Services، فتأكد من أنك تستخدم تحديثا حديثا [للموصلات العامة.](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history)
3. إذا توقف تشغيل مزامنة MIM مع وجود [](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) خطأ، فاستشارة جدول رموز خطأ التشغيل لتحديد الأسباب المحتملة.
4. إذا توقف التشغيل مع استثناء ملحق **dll،** انقر فوق  هذه الكلمات لفتح نافذة خصائص "كائن المسافة للموصل"، وانقر فوق "تتبع المكدس"... للاطلاع على مزيد من المعلومات حول السبب الأساسي، كما هو موضح في [Extension-DLL-Exception.](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx) 
5. إذا كان مكون خدمة الإعلام بتغيير كلمة المرور (PCNS) يظهر الخطأ **6025** في سجل الأحداث أثناء مزامنة كلمة المرور، فتحقق من دليل استكشاف أخطاء إرسال تقرير PCNS وإصلاحها [6025.](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx)
6. إذا كانت المزامنة الكاملة مع عامل إدارة خدمات  FIM بطيئة، فتحقق من إعداد النمو التلقائي ل TempDB، كما هو موضح في استكشاف الأخطاء وإصلاحها بالمزامنة الكاملة البطيئة أو [المعلقة.](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx)
7. إذا كنت تواجه خطأ خادم متوقف مع خدمات فشل الإنشاء عبر الويب باستخدام عامل إدارة خدمات FIM، فشاهد ["معلومات الدعم": فشل إنشاء-عبر-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) للحصول على نظرة عامة حول الأسباب.

