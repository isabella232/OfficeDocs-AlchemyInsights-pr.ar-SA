---
title: حدث خطا في التحقق من صحة خطا الرمز المميز للوصول اثناء تحليلات سطح المكتب علي البواردينج
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
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783538"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="d0922-102">ظهور رسالة الخطا "حدث خطا في التحقق من صحة الرمز المميز للوصول" اثناء إلحاق تحليلات سطح المكتب</span><span class="sxs-lookup"><span data-stu-id="d0922-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="d0922-103">هذا الخطا عاده ما يكون عند انتهاء صلاحيه رمز المصادقة.</span><span class="sxs-lookup"><span data-stu-id="d0922-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="d0922-104">يؤدي تحديث الصفحة عاده إلى تحديث الرمز المميز.</span><span class="sxs-lookup"><span data-stu-id="d0922-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="d0922-105">ومع ذلك ، يمكن ان تستمر هذه المشكلة في حاله وجود اي نهج وصول شرطي تم تطبيقه علي الحساب الذي يتم استخدامه لتحليلات سطح المكتب علي اللوحة.</span><span class="sxs-lookup"><span data-stu-id="d0922-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="d0922-106">يمكنك مراجعه سجلات تسجيل الدخول إلى Azure AD في مدخل Azure لمعرفه ما إذا كان هناك اي عمليات فشل في تسجيل الدخول إلى الحساب الذي يتم استخدامه للحاق تحليلات سطح المكتب.</span><span class="sxs-lookup"><span data-stu-id="d0922-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="d0922-107">لمزيد من المعلومات حول الوصول الشرطي ، تفضل بزيارة [تخطيط نشر Access الشرطي](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="d0922-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>