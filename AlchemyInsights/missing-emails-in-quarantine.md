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
ms.openlocfilehash: 563f76f624f428a46894268b478cf05eb757b497
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539811"
---
# <a name="missing-emails-in-quarantine"></a>رسائل البريد الإلكتروني المفقودة في الفحص"

يمكن للمسؤولين [عرض هذه الرسائل أو إصدارها أو حذفها.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

لفتح مركز التوافق &، انتقل إلى [https://protection.office.com](https://protection.office.com/) . لفتح صفحة الفحص مباشرة، انتقل إلى [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

يمكنك البحث حسب القيم التالية:  

- **معرف الرسالة**: المعرف الفريد العام للرسالة. إذا حددت رسالة في القائمة، تظهر القيمة **"معرّف** الرسالة" في جزء القائمة من خلال التفاصيل التي تظهر.  يمكن للمسؤولين [استخدام تتبع الرسائل](/microsoft-365/security/office-365-security/message-trace-scc) للعثور على الرسائل وقيمها المطابقة لمعرف الرسالة.
- **عنوان البريد الإلكتروني المرسل:** عنوان البريد الإلكتروني لمرسل واحد.
- **عنوان البريد الإلكتروني للمستلم**: عنوان البريد الإلكتروني لمستلم واحد.
- **الموضوع**: استخدم الموضوع بالكامل للرسالة. لا يتحسس البحث حالة التحسس.

بعد إدخال معايير البحث، انقر فوق الزر ![ تحديث ](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **تحديث** لتصفية النتائج.

إن cmdlets التي تستخدمها لعرض الرسائل والملفات وإدارتها في الفحص هي:
- [Delete-QuarantineMessage](/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): لاحظ أن أمر cmdlet هذا للرسائل فقط، وليس ملفات البرامج الضارة من Microsoft Defender ل Office 365 ل SharePoint Online أو OneDrive for Business أو Teams.
- [Release-QuarantineMessage](/powershell/module/exchange/release-quarantinemessage)