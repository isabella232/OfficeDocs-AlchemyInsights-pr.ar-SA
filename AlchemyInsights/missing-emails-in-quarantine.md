---
title: رسائل البريد الإلكتروني المفقودة في الفحص
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831721"
---
# <a name="missing-emails-in-quarantine"></a>رسائل البريد الإلكتروني المفقودة في الفحص"

يمكن للمسؤولين [عرض هذه الرسائل أو إصدارها أو حذفها.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

لفتح مركز التوافق &، انتقل إلى [https://protection.office.com](https://protection.office.com/) . لفتح صفحة الفحص مباشرة، انتقل إلى [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

يمكنك البحث حسب القيم التالية:  

- **معرف الرسالة**: المعرف الفريد العام للرسالة. إذا حددت رسالة في القائمة، تظهر القيمة **"معرّف** الرسالة" في جزء القائمة من خلال التفاصيل التي تظهر.  يمكن للمسؤولين [استخدام تتبع الرسائل](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) للعثور على الرسائل وقيمها المطابقة لمعرف الرسالة.
- **عنوان البريد الإلكتروني المرسل:** عنوان البريد الإلكتروني لمرسل واحد.
- **عنوان البريد الإلكتروني للمستلم**: عنوان البريد الإلكتروني لمستلم واحد.
- **الموضوع**: استخدم الموضوع بالكامل للرسالة. لا يتحسس البحث حالة التحسس.

بعد إدخال معايير البحث، انقر فوق الزر ![ تحديث ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **تحديث** لتصفية النتائج.  

إن cmdlets التي تستخدمها لعرض الرسائل والملفات وإدارتها في الفحص هي:
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): لاحظ أن أمر cmdlet هذا للرسائل فقط، وليس ملفات البرامج الضارة من ATP ل SharePoint Online أو OneDrive for Business أو Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)