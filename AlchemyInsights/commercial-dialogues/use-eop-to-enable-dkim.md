---
title: استخدام Exchange Online PowerShell لتمكين DKIM لمجال معين
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: ba627c6da96624914b858aa09d6eff9de709134c2c986fe363845c5ab2b66434
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070275"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>استخدام Exchange Online PowerShell لتمكين DKIM لمجال معين

إذا لم تتمكن من إنشاء سجلات DNS ل DKIM في مركز الإدارة، فحاول استخدام Exchange Online PowerShell. 

لإنشاء سجل DNS DKIM باستخدام Exchange Online PowerShell، قم بتنفيذ الخطوات التالية:

1. افتح Windows PowerShell كمسؤول، ثم ادير الأوامر التالية بالتسلسل الموضح:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
إذا كنت تواجه مشكلة في الاتصال Exchange Online PowerShell، فشاهد الاتصال Exchange Online [PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

2. بمجرد الاتصال ب PowerShell، Exchange Online الأمر التالي:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. بمجرد تنفيذ الأمر أعلاه بنجاح، تشغيل الأمر التالي لإنهاء جلسة Exchange Online PowerShell:

    `Remove-PSSession $Session` 



