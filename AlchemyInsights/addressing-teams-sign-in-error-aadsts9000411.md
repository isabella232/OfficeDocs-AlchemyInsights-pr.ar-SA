---
title: خطأ تسجيل الدخول إلى Teams AADSTS9000411
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821974"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="e2441-102">خطأ تسجيل الدخول إلى Teams AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="e2441-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="e2441-103">عند تسجيل الدخول إلى Microsoft Teams، قد تتلقى رسالة الخطأ: عذرا، ولكننا نواجه مشكلة في تسجيل الدخول في **AADSTS9000411: لم يتم تنسيق الطلب بشكل صحيح. يتم تكرار المعلمة "login_hint".**</span><span class="sxs-lookup"><span data-stu-id="e2441-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="e2441-104">لمعالجة هذه المشكلة، يرجى التأكد من تحديث عملاء Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e2441-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="e2441-105">لمزيد من المعلومات حول تحديث العميل، راجع [تحديث Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="e2441-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="e2441-106">إذا لم تتمكن من تحديث العميل لسبب ما، فإن تسجيل الخروج من العميل سيمسح معظم البيانات المخزنة مؤقتا.</span><span class="sxs-lookup"><span data-stu-id="e2441-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="e2441-107">ومع ذلك، إذا كانت لا تزال لديك مشاكل بعد تسجيل/تسجيل، فتوقف عن Teams ويرجى مسح ذاكرة التخزين المؤقت للعميل من خلال القيام بما يلي:</span><span class="sxs-lookup"><span data-stu-id="e2441-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="e2441-108">أغلق Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e2441-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="e2441-109">انتقل إلى: ٪appdata٪\microsoft\teams واحذف كل الملفات.</span><span class="sxs-lookup"><span data-stu-id="e2441-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="e2441-110">أعد فتح Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e2441-110">Reopen Microsoft Teams.</span></span>
