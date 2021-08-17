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
ms.openlocfilehash: 12751288d04a2ec5993bf4a546b7d0c862f8f171f5bfd7a337cb79cb95792056
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040817"
---
# <a name="password-policies"></a>سياسات كلمات المرور

**أواجه مشاكل في نهج كلمة المرور للمستخدم**

- يعتمد نهج كلمة المرور للمستخدم على ما إذا كان المستخدم في السحابة فقط أو في الموقع.
- يجب على المستخدمين في السحابة فقط اختيار كلمة مرور تفي بالمتطلبات في هذه المقالة: سياسات كلمات المرور التي تنطبق فقط على حسابات [المستخدمين في السحابة](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)
- يجب على المستخدمين في الموقع اختيار كلمة مرور تلبي المتطلبات المحلية. إذا تعذر على المستخدمين في الموقع تعيين كلمة المرور الخاصة بهم، فتحقق من متطلباتك المحلية.

**لا أعرف كيفية تعيين أو التحقق من سياسات انتهاء صلاحية كلمة المرور**

- يمكنك تعيين نهج انتهاء الصلاحية والتحقق منه لمستخدمي السحابة في المستأجر باستخدام PowerShell. اتبع الإرشادات الواردة في هذه المقالة: تعيين سياسات كلمات المرور أو التحقق [منها باستخدام PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- يتم تعيين نهج انتهاء صلاحية كلمة المرور للمستخدمين في الموقع في AD الخاص بك.

**ارتباطات مفيدة أخرى:**
- [بدء استخدام إعادة تعيين كلمة المرور](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [استكشاف مشاكل إعادة تعيين كلمة المرور التي بدأها المسؤول وإصلاحها](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
