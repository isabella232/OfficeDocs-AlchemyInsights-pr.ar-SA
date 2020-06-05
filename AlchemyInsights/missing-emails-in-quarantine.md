---
title: رسائل البريد الإلكتروني المفقودة في الحجر الصحي
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/03/2020
ms.locfileid: "44568890"
---
# <a name="missing-emails-in-quarantine"></a>رسائل البريد الإلكتروني المفقودة في الحجر الصحي"

يمكن للمسؤولين [عرض هذه الرسائل أو إصدارها أو حذفها.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

لفتح مركز التوافق & الأمان، انتقل إلى [https://protection.office.com](https://protection.office.com/) . لفتح صفحة الحجر الصحي مباشرة، انتقل إلى [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

يمكنك البحث حسب القيم التالية:  

- **معرف الرسالة:** المعرف الفريد للرسالة بشكل عام. إذا قمت بتحديد رسالة في القائمة، تظهر قيمة **معرف الرسالة** في جزء **التفاصيل** المنبثقة الذي يظهر. يمكن للمسؤولين استخدام [تتبع الرسائل](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) للعثور على الرسائل وقيم معرّف الرسائل المقابلة لها.
- **عنوان البريد الإلكتروني للمرسل:** عنوان البريد الإلكتروني لمرسل واحد.
- **عنوان البريد الإلكتروني للمستلم:** عنوان البريد الإلكتروني لمستلم واحد.
- **الموضوع**: استخدم موضوع الرسالة بأكمله. البحث ليس حساساً للحالة.

بعد إدخال معايير البحث، انقر فوق ![ تحديث زر ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **التحديث** لتصفية النتائج.  

cmdlets التي تستخدمها لعرض وإدارة الرسائل والملفات في الحجر الصحي هي:
- [حذف-العزلرسالة](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [رسالة التصدير والحجر الصحي](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [الحصول على الحجر الصحيرسالة](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [معاينة الحجرالصحيرسالة](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): لاحظ أن هذا cmdlet هو فقط للرسائل ، وليس ملفات البرامج الضارة من ATP لSharePoint أون لاين ، OneDrive للأعمال التجارية ، أو فرق.
- [رسالة الإصدار-الحجر الصحي](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)