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
ms.openlocfilehash: 21f80a7cc8b00ac56acdb05add1e1bfdfac9d827
ms.sourcegitcommit: c061f1dfa6f557a9ec083dd030b73b121d9864ea
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/14/2020
ms.locfileid: "43286235"
---
# <a name="change-strong-password-requirement"></a>تغيير متطلبات كلمة المرور القوية

تتطلب Microsoft كلمات مرور قوية بشكل افتراضي. 

باستخدام PowerShell، يمكنك تعطيل كلمات مرور قوية لمستخدمين محددين بهذا الأمر:<br>
*تعيين MsolUser - UserPrincipalName <UserPrincipalName> - StrongPasswordRequired $false*

- [مزيد من المعلومات حول نهج كلمة المرور](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [كيفية الاتصال بـ Office 365 باستخدام PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [مزيد من المعلومات حول أوامر PowerShell MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
- [تعيين كلمة مرور مستخدم فردي إلى عدم انتهاء صلاحيتها](https://docs.microsoft.com/microsoft-365/admin/add-users/set-password-to-never-expire)
