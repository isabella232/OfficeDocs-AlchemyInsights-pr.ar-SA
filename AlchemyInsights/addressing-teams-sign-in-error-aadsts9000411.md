---
title: معالجة فرق تسجيل الدخول خطأ AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: b70f1320ea1dfa29e6fa489bd02acfcd1d92971b
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357259"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="3ff5c-102">معالجة فرق تسجيل الدخول خطأ AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="3ff5c-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="3ff5c-103">عند تسجيل الدخول إلى Microsoft Teams، قد تتلقى الخطأ: **عذراً، ولكن نا جناً مشكلة في تسجيل الدخول في AADSTS9000411: لم يتم تنسيق الطلب بشكل صحيح. يتم تكرار المعلمة "login_hint".**</span><span class="sxs-lookup"><span data-stu-id="3ff5c-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="3ff5c-104">لمعالجة هذه المشكلة، الرجاء التأكد من تحديث عملاء Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="3ff5c-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="3ff5c-105">لمزيد من المعلومات حول تحديث عميلك، راجع [تحديث فرق Microsoft](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="3ff5c-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="3ff5c-106">إذا لم تتمكن من تحديث العميل لسبب ما، سيؤدي تسجيل الخروج من العميل إلى مسح معظم البيانات المخزنة مؤقتًا.</span><span class="sxs-lookup"><span data-stu-id="3ff5c-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="3ff5c-107">ومع ذلك، إذا كان لا يزال لديك مشاكل بعد تسجيل الخروج/تسجيل الدخول، إنهاء فرق الرجاء مسح ذاكرة التخزين المؤقت العميل الخاص بك عن طريق القيام بما يلي:</span><span class="sxs-lookup"><span data-stu-id="3ff5c-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="3ff5c-108">إغلاق فرق Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3ff5c-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="3ff5c-109">انتقل إلى: %appdata%\microsoft\teams وحذف كافة الملفات.</span><span class="sxs-lookup"><span data-stu-id="3ff5c-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="3ff5c-110">إعادة فتح فرق Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3ff5c-110">Reopen Microsoft Teams.</span></span>
