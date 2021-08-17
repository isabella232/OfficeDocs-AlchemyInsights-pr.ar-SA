---
title: 1385-Office-365-alert-policies
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: 681f7609f32b004ddfa7bfbeff179757e7063657
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58312674"
---
# <a name="alert-policies"></a>سياسات التنبيه

Microsoft 365 على سياسات [](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) تنبيه افتراضية تؤدي إلى تشغيل تنبيهات المؤسسات التي تتضمن اشتراكا في Microsoft 365 Enterprise أو Microsoft 365 US Government E1/G1 أو E3/G3 أو E5/G5. وبالتالي، قد يتلقى المسؤولون إعلاما بالبريد الإلكتروني للتنبيه تم إرساله بواسطة Office365Alerts@microsoft.com سطر موضوع مثل "تنبيه منخفض *الخطورة:* اسم نهج التنبيه". يتم إرسال إعلامات التنبيهات عند تشغيل التنبيهات الخاصة بالأنشطة الشائعة، على سبيل المثال عند المستخدمين:

- إنشاء قواعد علبة الوارد التي تقوم ب إعادة توجيه البريد الإلكتروني.
- تعيين الأذونات لعلبة البريد الخاصة بهم.
- مشاركة عدد كبير من الملفات أو حذفها في SharePoint الملفات.
- إنشاء عمليات بحث eDiscovery وتصدير نتائج البحث.

لمراجعة تنبيه والتصرف فيه:

1. القيام بوا واحدة من الخطوات التالية:
   - في مركز التوافق في Microsoft 365 في <https://compliance.microsoft.com> ، انتقل إلى **تنبيهات**. أو، انتقل مباشرة إلى صفحة **التنبيهات،** استخدم <https://compliance.microsoft.com/compliancealerts> .
   - في مدخل Microsoft 365 Defender في ، انتقل إلى الأحداث <https://security.microsoft.com> **&** \> **تنبيهات التنبيهات**. أو، انتقل مباشرة إلى صفحة **التنبيهات،** استخدم <https://security.microsoft.com/alerts> .
2. انقر فوق تنبيه لعرض صفحة منبهة تحتوي على معلومات حول التنبيه.

يمكنك اتخاذ إجراء على تنبيه، مثل إزالة قاعدة علبة وارد [مريبة](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account). أو يمكنك ببساطة إغلاق التنبيه عن طريق النقر فوق **حل** على صفحة منبه منبه.

لمزيد من المعلومات حول تكوين سياسات التنبيهات وإدارتها، راجع  [هذه المقالة](https://docs.microsoft.com/microsoft-365/compliance/alert-policies).

**هام**: تنبيه إعلامات البريد الإلكتروني من Microsoft لن يطلب منك أبدا القيام ب التالي:

- توفير كلمة مرور
- التحقق من تفاصيل الأمان لحسابك
- إعادة المصادقة بنفسك

إذا تلقيت رسالة بريد إلكتروني بها هذه الأنواع من الطلبات، فإن Microsoft لم ترسلها ويجب أن تعتبر رسالة تصيد احتيالي احتيالية. إذا تلقيت رسالة بهذه الأنواع من الطلبات، ف الإبلاغ [عن الرسالة إلى Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft).
