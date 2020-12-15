---
title: تسجيل الدخول إلى Microsoft Edge تلقائيا
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/08/2020
ms.locfileid: "49676705"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="f046b-102">تسجيل الدخول إلى Microsoft Edge تلقائيا</span><span class="sxs-lookup"><span data-stu-id="f046b-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="f046b-103">يستخدم Microsoft Edge حساب نظام التشغيل الافتراضي لتسجيل الدخول تلقائيا إلى المستخدم وفقا لكيفيه تكوين جهاز المستخدم.</span><span class="sxs-lookup"><span data-stu-id="f046b-103">Microsoft Edge uses the OS's default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="f046b-104">يتم وصف سيناريوهات كل نوع من أنواع تكوين الاجهزه وعمليه تسجيل الدخول التابعة له للمستخدم أدناه:</span><span class="sxs-lookup"><span data-stu-id="f046b-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

1. <span data-ttu-id="f046b-105">**الجهاز مختلط/AAD-J**: يتوفر هذا الخيار علي نظام التشغيل windows 10 والمستوي الأدنى لنظام التشغيل windows وإصدارات خوادم مقابله.</span><span class="sxs-lookup"><span data-stu-id="f046b-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="f046b-106">يقوم المستخدمون بتسجيل الدخول تلقائيا باستخدام حسابات Azure Active directory (AD) الخاصة بهم.</span><span class="sxs-lookup"><span data-stu-id="f046b-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
2. <span data-ttu-id="f046b-107">**الجهاز مرتبط بالمجال**: يتوفر هذا الخيار علي نظام التشغيل windows 10 والمستوي الأدنى لنظام التشغيل windows وإصدارات خوادم مقابله.</span><span class="sxs-lookup"><span data-stu-id="f046b-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="f046b-108">بشكل افتراضي ، لا يتم تسجيل دخول المستخدمين الذين لديهم حسابات المجالات تلقائيا ؛ لتمكين تسجيل الدخول التلقائي لهم ، استخدم نهج **كونفيجوريونبريميسيساككونتاوتوسيجنين** .</span><span class="sxs-lookup"><span data-stu-id="f046b-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="f046b-109">لتمكين تسجيل الدخول التلقائي للمستخدمين الذين لديهم حسابات Azure AD ، خذ في الاعتبار الانضمام المختلط إلى أجهزتهم.</span><span class="sxs-lookup"><span data-stu-id="f046b-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
3. <span data-ttu-id="f046b-110">**الحساب الافتراضي لنظام التشغيل هو حساب Microsoft**: يتوفر هذا الخيار علي WINDOWS 10 RS3 (الإصدار 1709 والإنشاء 10.0.16299) والإصدارات الأحدث.</span><span class="sxs-lookup"><span data-stu-id="f046b-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="f046b-111">هذا السيناريو من المحتمل حدوثه علي أجهزه المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="f046b-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="f046b-112">ومع ذلك ، إذا كان الحساب الافتراضي لنظام التشغيل هو حساب Microsoft ، سيقوم Microsoft Edge تلقائيا بتسجيل الدخول إلى المستخدم باستخدام حساب Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f046b-112">However, if the OS's default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
