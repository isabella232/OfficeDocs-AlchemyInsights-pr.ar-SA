---
title: إصلاح مشاكل اعداد الأشرف
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
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744937"
---
# <a name="fix-dkim-setup-issues"></a>إصلاح مشاكل اعداد الأشرف

إذا واجهت مشاكل في تمكين DKIM لمجالك المخصص ، فاتبع الخطوات التالية:

- ترتبط معظم مشاكل اعداد DKIM بسجلات DNS غير الصحيحة. تاكد من تنسيق السجل الخاص ب DKIM CNAME (**وليس** سجل TXT) بشكل صحيح. لمزيد من المعلومات ، راجع هذا [الموضوع](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- بعد إنشاء سجلات DNS الخاصة ب DKIM أو تحديثها في خدمه استضافه DNS لمجالك (عاده ما يكون جهة تسجيل المجالات الخاصة بك) ، انتظر حتى يتم نشر سجلات DNS.

- إذا لم تتمكن من إنشاء سجلات DNS ل DKIM في مركز الاداره ، فيمكنك استبدالها \<CustomDomain\> بمجالك المخصص (علي سبيل المثال ، contoso.com) وتشغيل هذا الأمر في [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
