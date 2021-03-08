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
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a><span data-ttu-id="7cec4-102">استخدام Exchange Online PowerShell لتمكين DKIM لمجال معين</span><span class="sxs-lookup"><span data-stu-id="7cec4-102">Use Exchange Online PowerShell to enable DKIM for a specific domain</span></span>

<span data-ttu-id="7cec4-103">إذا لم تتمكن من إنشاء سجلات DNS ل DKIM في مركز الإدارة، فحاول استخدام Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="7cec4-103">If you can't create the DKIM DNS records in the admin center, try using Exchange Online PowerShell.</span></span> 

<span data-ttu-id="7cec4-104">لإنشاء سجل DNS ل DKIM باستخدام Exchange Online PowerShell، قم بتنفيذ الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="7cec4-104">To create a DKIM DNS record using Exchange Online PowerShell, perform the following steps:</span></span>

1. <span data-ttu-id="7cec4-105">افتح Windows PowerShell كمسؤول وتولى تشغيل الأوامر التالية بالتسلسل الموضح:</span><span class="sxs-lookup"><span data-stu-id="7cec4-105">Open Windows PowerShell as an administrator and run the following commands in the described sequence:</span></span>

    <span data-ttu-id="7cec4-106">أ.</span><span class="sxs-lookup"><span data-stu-id="7cec4-106">a.</span></span> `$UserCredential = Get-Credential`

    <span data-ttu-id="7cec4-107">ب.</span><span class="sxs-lookup"><span data-stu-id="7cec4-107">b.</span></span> `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="7cec4-108">ج.</span><span class="sxs-lookup"><span data-stu-id="7cec4-108">c.</span></span> `Import-PSSession $Session -DisableNameChecking`
    
<span data-ttu-id="7cec4-109">إذا كنت تواجه مشكلة في الاتصال ب Exchange Online PowerShell، فشاهد [الاتصال ب Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)</span><span class="sxs-lookup"><span data-stu-id="7cec4-109">If you have trouble connecting to Exchange Online PowerShell, see [Connect to Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="7cec4-110">بمجرد اتصالك ب Exchange Online PowerShell، يمكنك تشغيل الأمر التالي:</span><span class="sxs-lookup"><span data-stu-id="7cec4-110">Once you're connected to Exchange Online PowerShell, run the following command:</span></span>

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. <span data-ttu-id="7cec4-111">بمجرد تنفيذ الأمر أعلاه بنجاح، تشغيل الأمر التالي لإنهاء جلسة عمل Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="7cec4-111">Once the above command has been successfully executed, run the following command to terminate the Exchange Online PowerShell session:</span></span>

    `Remove-PSSession $Session` 



