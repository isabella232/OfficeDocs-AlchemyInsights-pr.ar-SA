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
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398716"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="8b9ac-102">تسجيل الدخول إلى Microsoft Edge تلقائيا</span><span class="sxs-lookup"><span data-stu-id="8b9ac-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="8b9ac-103">يستخدم Microsoft Edge الحساب الافتراضي ل OS تسجيل الدخول إلى المستخدم تلقائيا وفقا لكيفية تكوين جهاز المستخدم.</span><span class="sxs-lookup"><span data-stu-id="8b9ac-103">Microsoft Edge uses the OS default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="8b9ac-104">يتم وصف سيناريوهات كل نوع من أنواع تكوين الجهاز وعملية تسجيل الدخول التابعة للمستخدم أدناه:</span><span class="sxs-lookup"><span data-stu-id="8b9ac-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

- <span data-ttu-id="8b9ac-105">**الجهاز مختلط/AAD-J**: يتوفر هذا الخيار على Windows 10، و Windows بمستوى أدنى، والإصدارات المقابلة من الخادم.</span><span class="sxs-lookup"><span data-stu-id="8b9ac-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="8b9ac-106">يتم تسجيل الدخول تلقائيا إلى المستخدمين باستخدام حسابات Azure Active Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="8b9ac-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
- <span data-ttu-id="8b9ac-107">**الجهاز منضم إلى** المجال : يتوفر هذا الخيار على Windows 10، و Windows بمستوى أدنى، والإصدارات المقابلة من الخادم.</span><span class="sxs-lookup"><span data-stu-id="8b9ac-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="8b9ac-108">بشكل افتراضي، لا يتم تسجيل الدخول تلقائيا إلى المستخدمين الذين لديهم حسابات مجالات؛ لتمكين تسجيل الدخول التلقائي لهم، استخدم النهج **ConfigureOnPremisesAccountAutoSignIn.**</span><span class="sxs-lookup"><span data-stu-id="8b9ac-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="8b9ac-109">لتمكين تسجيل الدخول التلقائي للمستخدمين الذين لديهم حسابات Azure AD، يمكنك الانضمام المختلط إلى أجهزتهم.</span><span class="sxs-lookup"><span data-stu-id="8b9ac-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
- <span data-ttu-id="8b9ac-110">**الحساب الافتراضي لنظام** التشغيل هو حساب Microsoft : يتوفر هذا الخيار على Windows 10 RS3 (الإصدار 1709، النسخة 10.0.16299) والإصدارات الأحدث.</span><span class="sxs-lookup"><span data-stu-id="8b9ac-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="8b9ac-111">من غير المحتمل أن يحدث السيناريو على أجهزة المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="8b9ac-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="8b9ac-112">ومع ذلك، إذا كان حساب نظام التشغيل الافتراضي هو حساب Microsoft، فإن Microsoft Edge سي سجل الدخول تلقائيا إلى المستخدم باستخدام حساب Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8b9ac-112">However, if the OS default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
