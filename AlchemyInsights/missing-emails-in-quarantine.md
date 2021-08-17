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
ms.openlocfilehash: bd5a04fd5abad962b4e85e009a9232e1a93219c238c629506df5cfb034453df2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/11/2021
ms.locfileid: "57892034"
---
# <a name="missing-emails-in-quarantine"></a>رسائل البريد الإلكتروني المفقودة في الفحص

يمكن للمسؤولين [عرض هذه الرسائل أو تحريرها أو حذفها](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

في مدخل Microsoft 365 Defender في <https://security.microsoft.com> ، انتقل إلى **مراجعة** \> **الفحص**. أو، انتقل مباشرة إلى صفحة **الفحص،** استخدم <https://security.microsoft.com/quarantine> .  

لمزيد من المعلومات حول قيم البحث/التصفية التي يمكنك استخدامها، راجع إدارة الرسائل والملفات المعزولة [كمسؤول في EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files).

إن cmdlets التي تستخدمها لعرض الرسائل والملفات وإدارتها في الفحص هي:

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): لاحظ أن أمر cmdlet هذا هو فقط للرسائل، وليس الملفات من مرفقات خزينة للرسائل SharePoint أو OneDrive أو Microsoft Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
