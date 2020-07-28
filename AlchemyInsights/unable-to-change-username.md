---
title: غير قادر على تغيير اسم المستخدم
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438723"
---
# <a name="unable-to-change-username"></a><span data-ttu-id="5d538-102">غير قادر على تغيير اسم المستخدم</span><span class="sxs-lookup"><span data-stu-id="5d538-102">Unable to change UserName</span></span>

<span data-ttu-id="5d538-103">في بعض الحالات، لا يتم نشر تغييرات UPN (UserPrincipalName) إلى مجموعة النظراء.</span><span class="sxs-lookup"><span data-stu-id="5d538-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="5d538-104">قد تتلقى أخطاء التحقق من الصحة في مدخل Office 365 أو قد لا تتمكن من تغيير اسم المستخدم أو عنوان البريد الإلكتروني.</span><span class="sxs-lookup"><span data-stu-id="5d538-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="5d538-105">لحل هذه المشكلة، يدوياً تعيين UserPrincipalName باستخدام هذا الأمر PowerShell.</span><span class="sxs-lookup"><span data-stu-id="5d538-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="5d538-106">**مثال: إعادة تسمية مستخدم**</span><span class="sxs-lookup"><span data-stu-id="5d538-106">**Example: Rename a user**</span></span>

<span data-ttu-id="5d538-107">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="5d538-107">PowerShellCopy</span></span>

<span data-ttu-id="5d538-108">PS C: \> تعيين MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com"-NewUserPrincipalName "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="5d538-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="5d538-109">يعيد هذا الأمر تسمية davidc@contoso.com إلى davidchew@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="5d538-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="5d538-110">لمزيد من المعلومات، راجع [تعيين MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span><span class="sxs-lookup"><span data-stu-id="5d538-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>