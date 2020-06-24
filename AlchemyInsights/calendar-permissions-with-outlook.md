---
title: أذونات التقويم
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862024"
---
# <a name="calendar-permissions"></a>أذونات التقويم

يمكن للمستخدمين تغيير أذونات التقويم الخاصة بهم مع Outlook على ويب أو عملاء آخرين، ولكن كمسؤول قد تحتاج إلى التحقق أيضاً.  
مع Cmdlet Exchange PowerShell سوف تظهر لك الإذن على تقويم المستخدم:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

للاطلاع على مزيد من المعلومات، راجع ما يلي:

- [الحصول على علبة البريد مجلد](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [مجموعة علبة البريد مجلد](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [إضافة علبة بريد مجلد](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

يتم استخدام أذونات التقويم في مشاركة التقويمات، لمشاهدة مزيد من المعلومات حول مشاركة تقويم Outlook، راجع المقالات التالية:

- [مشاركة تقويم Outlook مع أشخاص آخرين](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [مشاركة التقويم الخاص بك في Outlook على الويب للأعمال](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

لاستكشاف "إذن التقويم" يمكنك استخدام أداة ["مساعد الدعم والاسترداد".](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f)