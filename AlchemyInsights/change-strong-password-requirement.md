---
title: تغيير متطلبات كلمة مرور قوية
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 8a82c002bd64a33556b632545e98355e860848d845e122bfea06fbc5ee5dcb90
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070671"
---
# <a name="change-strong-password-requirement"></a>تغيير متطلبات كلمة المرور القوية

تتطلب Microsoft كلمات مرور قوية بشكل افتراضي.

باستخدام PowerShell، يمكنك تعطيل كلمات مرور قوية لمستخدمين محددين باستخدام هذه الأوامر:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

لتعطيل كلمات مرور قوية لجميع المستخدمين، استخدم:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [مزيد من المعلومات حول نهج كلمة المرور](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [كيفية الاتصال Microsoft 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [مزيد من المعلومات حول أوامر PowerShell MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
