---
title: حدث خطأ في التحقق من صحة رمز الوصول المميز أثناء "تحليلات سطح المكتب" على متن الطائرة
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
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813675"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="35303-102">رسالة الخطأ "حدث خطأ في التحقق من صحة رمز الوصول المميز" أثناء تشغيل "تحليلات سطح المكتب"</span><span class="sxs-lookup"><span data-stu-id="35303-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="35303-103">يتم ملاحظة هذا الخطأ عادة عند انتهاء صلاحية رمز المصادقة المميز.</span><span class="sxs-lookup"><span data-stu-id="35303-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="35303-104">عادة، يحدث تحديث الصفحة الرمز المميز.</span><span class="sxs-lookup"><span data-stu-id="35303-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="35303-105">ومع ذلك، يمكن أن تستمر هذه المشكلة إذا كانت هناك أي سياسات وصول شرطي مطبقة على الحساب المستخدم في تحليلات سطح المكتب على اللوحة.</span><span class="sxs-lookup"><span data-stu-id="35303-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="35303-106">يمكنك مراجعة سجلات تسجيل الدخول إلى Azure AD في مدخل Azure لمعرفة ما إذا كان هناك أي حالات فشل في تسجيل الدخول للحساب الذي يتم استخدامه لتكمبيوتر "تحليلات سطح المكتب".</span><span class="sxs-lookup"><span data-stu-id="35303-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="35303-107">لمزيد من المعلومات حول الوصول الشرطي، تفضل بزيارة [تخطيط نشر الوصول الشرطي.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)</span><span class="sxs-lookup"><span data-stu-id="35303-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>