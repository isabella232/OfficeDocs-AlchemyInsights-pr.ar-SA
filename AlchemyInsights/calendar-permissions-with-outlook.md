---
title: أذونات التقويم
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: cfee520e26587c0a649c08084853c31232d027f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748780"
---
# <a name="calendar-permissions"></a>أذونات التقويم

يمكن للمستخدمين تغيير أذونات التقويم الخاصة بهم باستخدام Outlook علي الويب أو العملاء الآخرين ، ولكن كمسؤول قد تحتاج إلى التحقق منه أيضا.  
باستخدام Exchange PowerShell cmdlet سيعرض لك الاذن في تقويم المستخدم:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

للاطلاع علي مزيد من المعلومات ، راجع ما يلي:

- [مايلبوكسفولديربيرميسيون](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [ميلبوكسفولديربيرميشن](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [الوظائف الاضافيه ميلبوكسفولديربيرميشن](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

يتم استخدام أذونات التقويم في مشاركه التقويمات ، للاطلاع علي مزيد من المعلومات حول مشاركه تقويم Outlook ، راجع المقالات التالية:

- [مشاركة تقويم Outlook مع أشخاص آخرين](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [مشاركه التقويم في Outlook علي الويب للاعمال](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

لاستكشاف أخطاء التقويم وإصلاحها ، يمكنك استخدام أداه [مساعد الإصلاح والدعم](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) .