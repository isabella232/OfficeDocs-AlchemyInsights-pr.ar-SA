---
title: سياسات كلمات المرور
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 826e266d08aa68c0d4213d8058a0244f404fe965
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50742928"
---
# <a name="password-policies"></a><span data-ttu-id="72cc3-102">سياسات كلمات المرور</span><span class="sxs-lookup"><span data-stu-id="72cc3-102">Password policies</span></span>

<span data-ttu-id="72cc3-103">**أواجه مشاكل في نهج كلمة المرور للمستخدم**</span><span class="sxs-lookup"><span data-stu-id="72cc3-103">**I'm having problems with the password policy for a user**</span></span>

- <span data-ttu-id="72cc3-104">يعتمد نهج كلمة المرور للمستخدم على ما إذا كان المستخدم في السحابة فقط أو في الموقع.</span><span class="sxs-lookup"><span data-stu-id="72cc3-104">The password policy for a user depends on whether the user is cloud only or on-premises.</span></span>
- <span data-ttu-id="72cc3-105">يجب على المستخدمين في السحابة فقط اختيار كلمة مرور تفي بالمتطلبات في هذه المقالة: سياسات كلمات المرور التي تنطبق فقط على حسابات [المستخدمين في السحابة](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span><span class="sxs-lookup"><span data-stu-id="72cc3-105">Cloud only users must choose a password that meets the requirements in this article: [Password policies that only apply to cloud user accounts](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span></span>
- <span data-ttu-id="72cc3-106">يجب على المستخدمين في الموقع اختيار كلمة مرور تلبي المتطلبات المحلية.</span><span class="sxs-lookup"><span data-stu-id="72cc3-106">On-premises users must choose a password that meets the on-premises requirements.</span></span> <span data-ttu-id="72cc3-107">إذا تعذر على المستخدمين في الموقع تعيين كلمة المرور الخاصة بهم، فتحقق من متطلباتك المحلية.</span><span class="sxs-lookup"><span data-stu-id="72cc3-107">If an on-premises user is unable to set their password, check your on-premises requirements.</span></span>

<span data-ttu-id="72cc3-108">**لا أعرف كيفية تعيين أو التحقق من سياسات انتهاء صلاحية كلمة المرور**</span><span class="sxs-lookup"><span data-stu-id="72cc3-108">**I don't know how to set or check password expiration policies**</span></span>

- <span data-ttu-id="72cc3-109">يمكنك تعيين نهج انتهاء الصلاحية والتحقق منه لمستخدمي السحابة في المستأجر باستخدام PowerShell.</span><span class="sxs-lookup"><span data-stu-id="72cc3-109">You can set and check the expiration policy for cloud users in your tenant by using PowerShell.</span></span> <span data-ttu-id="72cc3-110">اتبع الإرشادات الواردة في هذه المقالة: تعيين سياسات كلمات المرور أو التحقق [منها باستخدام PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span><span class="sxs-lookup"><span data-stu-id="72cc3-110">Follow the instructions in this article: [Set or check the password policies by using PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span></span>
- <span data-ttu-id="72cc3-111">يتم تعيين نهج انتهاء صلاحية كلمة المرور للمستخدمين في الموقع في AD الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="72cc3-111">The password expiration policy for on-premises users is set in your on-premises AD.</span></span>

<span data-ttu-id="72cc3-112">**ارتباطات مفيدة أخرى:**</span><span class="sxs-lookup"><span data-stu-id="72cc3-112">**Other Helpful links:**</span></span>
- [<span data-ttu-id="72cc3-113">بدء استخدام إعادة تعيين كلمة المرور</span><span class="sxs-lookup"><span data-stu-id="72cc3-113">Getting Started with Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [<span data-ttu-id="72cc3-114">استكشاف مشاكل إعادة تعيين كلمة المرور التي بدأها المسؤول وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="72cc3-114">Troubleshoot Administrator-initiated Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
