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
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523110"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>استخدام Exchange Online PowerShell لتمكين DKIM لمجال معين

إذا لم تتمكن من إنشاء سجلات DNS ل DKIM في مركز الإدارة، فحاول استخدام Exchange Online PowerShell. 

لإنشاء سجل DNS ل DKIM باستخدام Exchange Online PowerShell، قم بتنفيذ الخطوات التالية:

1. افتح Windows PowerShell كمسؤول وتولى تشغيل الأوامر التالية بالتسلسل الموضح:

    أ. `$UserCredential = Get-Credential`

    ب. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    ج. `Import-PSSession $Session -DisableNameChecking`
    
إذا كنت تواجه مشكلة في الاتصال ب Exchange Online PowerShell، فشاهد [الاتصال ب Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. بمجرد اتصالك ب Exchange Online PowerShell، يمكنك تشغيل الأمر التالي:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. بمجرد تنفيذ الأمر أعلاه بنجاح، تشغيل الأمر التالي لإنهاء جلسة عمل Exchange Online PowerShell:

    `Remove-PSSession $Session` 



