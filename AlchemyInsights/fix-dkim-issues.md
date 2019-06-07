---
title: إصلاح مشكلات إعداد DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764801"
---
# <a name="fix-dkim-setup-issues"></a>إصلاح مشكلات إعداد DKIM

إذا واجهت مشكلات تمكين DKIM للمجال المخصص الخاص بك، اتبع الخطوات التالية:

- ترتبط معظم مشاكل الإعداد DKIM سجلات DNS غير صحيحة. تحقق من تنسيق سجل DKIM CNAME (**لا** سجل TXT). لمزيد من المعلومات، راجع هذا [الموضوع](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- بعد أن تقوم بإنشاء أو تحديث سجلات DKIM DNS في DNS المجان للمجال الخاص بك (بشكل عام، مسجل النطاق)، انتظر حتى يتم نشر سجلات DNS.

- إذا لا يمكن إنشاء سجلات DKIM DNS في مركز مسؤول، يمكنك استبدال \<كوستومدومين\> مع المجال المخصص الخاص بك (على سبيل المثال، contoso.com) وتشغيل هذا الأمر في [PowerShell Exchange الفورية](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.
