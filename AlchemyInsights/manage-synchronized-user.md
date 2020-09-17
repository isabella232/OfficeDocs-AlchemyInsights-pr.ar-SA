---
title: أداره المستخدم المتزامن
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 53c188f6c6ab93bcc6f87d95717dc0d24d492bb7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47777664"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="b8821-102">تعذر تعيين عنوان البريد الكتروني الأساسي أو تغيير سمات المستخدم أو أزاله/حذف مستخدم متزامن</span><span class="sxs-lookup"><span data-stu-id="b8821-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="b8821-103">إذا تم تمكين مزامنة الدليل لبيئتك ، فلا يمكن تغيير بعض سمات المستخدمين أو الكائنات باستخدام مركز أداره Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="b8821-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="b8821-104">لأداره المستخدمين المتزامنين وكل السمات الخاصة بهم بالبالكامل ، استخدم "وحده التحكم في أداره المستخدمين المحليين" ل active directory (أدسييديت).</span><span class="sxs-lookup"><span data-stu-id="b8821-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="b8821-105">بدلا من ذلك ، يمكنك تغيير المستخدمين الفرديين أو السمات لمستخدمين متزامنين باستخدام powershell كما هو مبين في هذه الامثله الشائعة:</span><span class="sxs-lookup"><span data-stu-id="b8821-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
