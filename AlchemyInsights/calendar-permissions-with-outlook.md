---
title: أذونات التقويم
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
- "3800009"
- "611"
ms.openlocfilehash: 4bf7680a422f096401f0a87bccd1b8dd11f4489f882bcc06864e37d6a248438c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046091"
---
# <a name="calendar-permissions"></a>أذونات التقويم

يمكن للمستخدمين تغيير أذونات التقويم الخاصة بهم باستخدام Outlook على الويب أو عملاء آخرين، ولكن كمسؤول قد تحتاج إلى التحقق أيضا.  
باستخدام Exchange، سيعرض لك PowerShell cmdlet الإذن في تقويم المستخدم:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

لمعرفة المزيد من المعلومات، راجع ما يلي:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

يتم استخدام أذونات التقويم في مشاركة التقويمات، لرؤية مزيد من المعلومات حول مشاركة تقويم Outlook، راجع المقالات التالية:

- [مشاركة تقويم Outlook مع أشخاص آخرين](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [مشاركة التقويم في Outlook على ويب للأعمال](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

لا استكشاف الأخطاء في إذن التقويم وإصلاحها، يمكنك استخدام [مساعد الإصلاح والدعم](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) التقويم.