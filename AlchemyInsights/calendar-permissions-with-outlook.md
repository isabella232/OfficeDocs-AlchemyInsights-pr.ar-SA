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
ms.openlocfilehash: bbd49134bd4a4451649b76bb5f60b19065910cae
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819895"
---
# <a name="calendar-permissions"></a>أذونات التقويم

يمكن للمستخدمين تغيير أذونات التقويم الخاصة بهم باستخدام Outlook على الويب أو عملاء آخرين، ولكن كمسؤول قد تحتاج إلى التحقق أيضا.  
باستخدام Exchange PowerShell cmdlet، سيعرض لك الإذن في تقويم المستخدم:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

لمعرفة المزيد من المعلومات، راجع ما يلي:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

يتم استخدام أذونات التقويم في مشاركة التقويمات، لرؤية مزيد من المعلومات حول مشاركة تقويم Outlook، راجع المقالات التالية:

- [مشاركة تقويم Outlook مع أشخاص آخرين](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [مشاركة التقويم في Outlook على الويب للأعمال](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

لاسترجاع أذونات التقويم وإصلاحها، يمكنك استخدام أداة مساعد [الاسترداد](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) والدعم.