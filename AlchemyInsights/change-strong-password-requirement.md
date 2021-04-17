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
ms.openlocfilehash: cf5cab9a1c2dd4226997d93417dc7104347f8a6e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818455"
---
# <a name="change-strong-password-requirement"></a>تغيير متطلبات كلمة المرور القوية

تتطلب Microsoft كلمات مرور قوية بشكل افتراضي.

باستخدام PowerShell، يمكنك تعطيل كلمات مرور قوية لمستخدمين محددين باستخدام هذه الأوامر:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

لتعطيل كلمات مرور قوية لجميع المستخدمين، استخدم:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [مزيد من المعلومات حول نهج كلمة المرور](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [كيفية الاتصال ب Microsoft 365 باستخدام PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [مزيد من المعلومات حول أوامر PowerShell MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
