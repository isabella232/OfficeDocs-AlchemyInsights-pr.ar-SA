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
# <a name="change-strong-password-requirement"></a><span data-ttu-id="83aa5-102">تغيير متطلبات كلمة المرور القوية</span><span class="sxs-lookup"><span data-stu-id="83aa5-102">Change strong password requirement</span></span>

<span data-ttu-id="83aa5-103">تتطلب Microsoft كلمات مرور قوية بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="83aa5-103">Microsoft requires strong passwords by default.</span></span> 

<span data-ttu-id="83aa5-104">باستخدام PowerShell، يمكنك تعطيل كلمات مرور قوية لمستخدمين محددين بهذا الأمر:</span><span class="sxs-lookup"><span data-stu-id="83aa5-104">Using PowerShell, you can disable strong passwords for specific users with this command:</span></span><br>
<span data-ttu-id="83aa5-105">*تعيين MsolUser - UserPrincipalName <UserPrincipalName> - StrongPasswordRequired $false*</span><span class="sxs-lookup"><span data-stu-id="83aa5-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false*</span></span>

- [<span data-ttu-id="83aa5-106">مزيد من المعلومات حول نهج كلمة المرور</span><span class="sxs-lookup"><span data-stu-id="83aa5-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="83aa5-107">كيفية الاتصال بـ Office 365 باستخدام PowerShell</span><span class="sxs-lookup"><span data-stu-id="83aa5-107">How to connect to Office 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="83aa5-108">مزيد من المعلومات حول أوامر PowerShell MsolUser</span><span class="sxs-lookup"><span data-stu-id="83aa5-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
- [<span data-ttu-id="83aa5-109">تعيين كلمة مرور مستخدم فردي إلى عدم انتهاء صلاحيتها</span><span class="sxs-lookup"><span data-stu-id="83aa5-109">Set an individual user's password to never expire</span></span>](https://docs.microsoft.com/microsoft-365/admin/add-users/set-password-to-never-expire)
