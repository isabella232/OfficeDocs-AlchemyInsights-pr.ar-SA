---
title: إصلاح مشاكل إعداد DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 5a613321ed79e657350ec4d19b1f07ac0a091b227a8268c793a10edd9990d41f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945918"
---
# <a name="fix-dkim-setup-issues"></a>إصلاح مشاكل إعداد DKIM

إذا واجهت مشاكل في تمكين DKIM لمجالك المخصص، فاتبع الخطوات التالية:

- ترتبط معظم مشاكل إعداد DKIM بسجلات DNS غير الصحيحة. تحقق من تنسيق سجل DKIM CNAME **(وليس** سجل TXT) بشكل صحيح. لمزيد من المعلومات، راجع هذا [الموضوع](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- بعد إنشاء سجلات DNS DKIM أو تحديثها في خدمة استضافة DNS لمجالك (عادة، جهة تسجيل المجالات)، انتظر حتى يتم نشر سجلات DNS.

- إذا لم تتمكن من إنشاء سجلات DNS ل DKIM في مركز الإدارة، يمكنك استبدال مجالك المخصص (على سبيل المثال، contoso.com) وتشغيل هذا الأمر في \<CustomDomain\> [Exchange Online PowerShell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
