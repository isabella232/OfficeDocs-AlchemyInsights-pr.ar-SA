---
title: إصلاح مشكلات إعداد DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717549"
---
# <a name="fix-dkim-setup-issues"></a>إصلاح مشكلات إعداد DKIM

إذا واجهت مشكلات تمكين DKIM للمجال المخصص الخاص بك، استخدم الخطوات التالية:

- ترتبط معظم مشكلات إعداد DKIM بسجلات DNS غير صحيحة. تحقق من تنسيق سجل DKIM CNAME **(وليس** سجل TXT) بشكل صحيح. لمزيد من المعلومات، راجع هذا [الموضوع](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- بعد إنشاء سجلات Dns DKIM أو تحديثها في خدمة استضافة DNS لنطاقك (عادةً، مسجل النطاق الخاص بك)، انتظر حتى تنتشر سجلات DNS.

- إذا لم تتمكن من إنشاء سجلات Dns DKIM في \<مركز\> المسؤول، يمكنك استبدال CustomDomain بالمجال المخصص (على سبيل `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`المثال، contoso.com) وتشغيل هذا الأمر في Exchange Online [PowerShell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).
