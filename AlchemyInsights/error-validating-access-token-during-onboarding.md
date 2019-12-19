---
title: حدث خطا في التحقق من خطا الرمز المميز للوصول اثناء تحليلات سطح المكتب علي الصعود
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741106"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="77030-102">خطا "حدث خطا في التحقق من صحة الرمز المميز للوصول" اثناء اعداد "تحليلات سطح المكتب"</span><span class="sxs-lookup"><span data-stu-id="77030-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="77030-103">عاده ما يتم ملاحظه هذا الخطا عند انتهاء صلاحيه الرمز المميز للمصادقة.</span><span class="sxs-lookup"><span data-stu-id="77030-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="77030-104">عاده ، تحديث الصفحة تحديث الرمز المميز.</span><span class="sxs-lookup"><span data-stu-id="77030-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="77030-105">ومع ذلك ، يمكن ان تستمر هذه المشكلة إذا كان هناك اي نهج "الوصول المشروط" المطبقة علي الحساب المستخدمة علي متن "تحليلات سطح المكتب".</span><span class="sxs-lookup"><span data-stu-id="77030-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="77030-106">يمكنك مراجعه سجلات تسجيل الدخول إلى Azure AD في المدخل Azure لمعرفه ما إذا كان هناك اي فشل تسجيل الدخول للحساب المستخدم لاعداد "تحليلات سطح المكتب".</span><span class="sxs-lookup"><span data-stu-id="77030-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="77030-107">لمزيد من المعلومات حول "الوصول المشروط" ، قم بزيارة [خطه نشر "الوصول المشروط](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)".</span><span class="sxs-lookup"><span data-stu-id="77030-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>