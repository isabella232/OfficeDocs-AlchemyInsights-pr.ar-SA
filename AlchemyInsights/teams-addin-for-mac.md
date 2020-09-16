---
title: وظيفة الفرق الاضافيه ل Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 1e5f6d66386398ad8600f9383f9f7a1dcf0ce69f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670315"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="dc10f-102">وظيفة الفرق الاضافيه ل Mac</span><span class="sxs-lookup"><span data-stu-id="dc10f-102">Teams add-in for Mac</span></span>

<span data-ttu-id="dc10f-103">لاستكشاف الأخطاء وإصلاحها لمستخدمي نظام التشغيل الاضافيه لفرق العمل المفقودة ، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="dc10f-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="dc10f-104">**الخطوة 1:** إذا كان لديك Exchange المختلط محليا (2016 CU3 أو إصدار لاحق) ، فاستخدم الاداه Test-HMA.ps1 للتاكد من تكوين المصادقة الاضافيه المختلطة بشكل صحيح.</span><span class="sxs-lookup"><span data-stu-id="dc10f-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="dc10f-105">للحصول علي مزيد من المعلومات ، راجع [التحقق من صحة اعداد المصادقة الحديثة المختلط ل Outlook ل iOS و Android](https://aka.ms/AA980zq).</span><span class="sxs-lookup"><span data-stu-id="dc10f-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/AA980zq).</span></span>  

<span data-ttu-id="dc10f-106">**ملاحظه** استخدم تنسيق عنوان UPN (علي سبيل المثال ، [username@contoso.com](mailto:username@contoso.com)) ، وليس domain\username.</span><span class="sxs-lookup"><span data-stu-id="dc10f-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="dc10f-107">قم بذلك حتى للمستخدمين الذين لديهم علب بريد Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="dc10f-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="dc10f-108">**الخطوة 2:** اجعل المستخدم ينتقل إلى **Tools**  >  **أدوات الحسابات**... في Outlook for Mac ، وابحث عن الحساب وحدده.</span><span class="sxs-lookup"><span data-stu-id="dc10f-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="dc10f-109">قم بتاكيد اسم المستخدم المدرج بتنسيق UPN (علي سبيل المثال ، [username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="dc10f-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="dc10f-110">**الخطوة 3:** تاكد من ان المستخدم هو مستخدم لفرق Microsoft مرخص.</span><span class="sxs-lookup"><span data-stu-id="dc10f-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="dc10f-111">يجب ان يستخدم المستخدم اشتراك Office 365 for Mac أو إصدار المنتج 16.24 أو إصدار أحدث.</span><span class="sxs-lookup"><span data-stu-id="dc10f-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>