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
ms.openlocfilehash: c77da6716c0755d6ed4911f490e000bd74d08f92
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329649"
---
# <a name="missing-emails-in-quarantine"></a>رسائل البريد الإلكتروني المفقودة في الفحص

يمكن للمسؤولين [عرض هذه الرسائل أو تحريرها أو حذفها](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

في مدخل Microsoft 365 Defender في <https://security.microsoft.com> ، انتقل إلى **مراجعة** \> **الفحص**. أو، انتقل مباشرة إلى صفحة **الفحص،** استخدم <https://security.microsoft.com/quarantine> .  

لمزيد من المعلومات حول قيم البحث/التصفية التي يمكنك استخدامها، راجع إدارة الرسائل والملفات المعزولة [كمسؤول في EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files).

إن cmdlets التي تستخدمها لعرض الرسائل والملفات وإدارتها في الفحص هي:

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): لاحظ أن أمر cmdlet هذا للرسائل فقط، وليس الملفات من مرفقات خزينة ل SharePoint أو OneDrive أو Microsoft Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
