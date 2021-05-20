---
title: Teams الإضافية ل Mac
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
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582057"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="c1ffb-102">Teams الإضافية ل Mac</span><span class="sxs-lookup"><span data-stu-id="c1ffb-102">Teams add-in for Mac</span></span>

<span data-ttu-id="c1ffb-103">لا استكشاف الأخطاء وإصلاحها في Teams الإضافية لمستخدمي نظام التشغيل Mac، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="c1ffb-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="c1ffb-104">**الخطوة 1:** إذا كان لديك Exchange مختلط (2016 CU3 أو الإصدارات اللاحقة مطلوبة)، فاستخدم أداة Test-HMA.ps1 لتأكيد تكوين المصادقة الحديثة المختلطة بشكل صحيح.</span><span class="sxs-lookup"><span data-stu-id="c1ffb-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="c1ffb-105">لمزيد من المعلومات، راجع التحقق من صحة إعداد المصادقة الحديثة المختلطة [Outlook لنظامي التشغيل iOS وAndroid](https://aka.ms/TestHMAEAS).</span><span class="sxs-lookup"><span data-stu-id="c1ffb-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/TestHMAEAS).</span></span>  

<span data-ttu-id="c1ffb-106">**ملاحظة** استخدم تنسيق عنوان UPN (على سبيل [المثال، username@contoso.com)،](mailto:username@contoso.com)وليس domain\username.</span><span class="sxs-lookup"><span data-stu-id="c1ffb-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="c1ffb-107">يمكنك القيام بذلك حتى للمستخدمين الذين لديهم Exchange Online بريد.</span><span class="sxs-lookup"><span data-stu-id="c1ffb-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="c1ffb-108">**الخطوة 2:** هل تريد من المستخدم الانتقال إلى **أدوات**  >  **الحسابات**... في Outlook for Mac، واعثر على الحساب وحدده.</span><span class="sxs-lookup"><span data-stu-id="c1ffb-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="c1ffb-109">تأكد من أن اسم المستخدم المدرج بتنسيق UPN (على سبيل [المثال،](mailto:username@contoso.com)username@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="c1ffb-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="c1ffb-110">**الخطوة 3:** تأكد من أن المستخدم مستخدم Microsoft Teams مرخص.</span><span class="sxs-lookup"><span data-stu-id="c1ffb-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="c1ffb-111">يجب أن يستخدم المستخدم Office 365 for Mac، إصدار المنتج 16.24 أو إصدار أحدث.</span><span class="sxs-lookup"><span data-stu-id="c1ffb-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>