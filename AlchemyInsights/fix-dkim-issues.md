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
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506761"
---
# <a name="fix-dkim-setup-issues"></a>إصلاح مشكلات إعداد DKIM

إذا واجهت مشكلات تمكين DKIM للمجال المخصص الخاص بك، استخدم الخطوات التالية:

- ترتبط معظم مشكلات إعداد DKIM بسجلات DNS غير صحيحة. تحقق من تنسيق سجل DKIM CNAME **(وليس** سجل TXT) بشكل صحيح. لمزيد من المعلومات، راجع هذا [الموضوع](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- بعد إنشاء سجلات Dns DKIM أو تحديثها في خدمة استضافة DNS لنطاقك (عادةً، مسجل النطاق الخاص بك)، انتظر حتى تنتشر سجلات DNS.

- إذا لم تتمكن من إنشاء سجلات Dns DKIM في مركز المسؤول، يمكنك استبدال \<CustomDomain\> المجال المخصص (على سبيل المثال، contoso.com) وتشغيل هذا الأمر في [Exchange Online PowerShell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
