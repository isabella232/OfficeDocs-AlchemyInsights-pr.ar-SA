---
title: تغيير متطلبات كلمة المرور القوية
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: f8790a26ec7c5de57f5dbfc9e1c162767c599f03
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36518746"
---
# <a name="change-strong-password-requirement"></a>تغيير متطلبات كلمة المرور القوية

تتطلب Microsoft كلمات مرور قوية بشكل افتراضي. 

استخدام PowerShell، يمكنك تعطيل كلمات مرور قوية لمستخدمين محددين بهذا الأمر:<br>
*مجموعة مسولوسير-UserPrincipalName <UserPrincipalName> -سترونجباسووردريكويريد $false*

- [مزيد من المعلومات حول نهج كلمة المرور](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [كيفية الاتصال Office 365 مع PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [مزيد من المعلومات حول أوامر PowerShell مسولوسير](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)