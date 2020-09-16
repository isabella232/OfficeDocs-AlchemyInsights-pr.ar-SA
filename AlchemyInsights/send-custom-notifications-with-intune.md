---
title: إرسال اعلامات مخصصه باستخدام Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720633"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="804f3-102">كيفيه إرسال اعلامات مخصصه إلى مستخدمي نظام التشغيل iOS و Android المدارين</span><span class="sxs-lookup"><span data-stu-id="804f3-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="804f3-103">تتم معالجه الإشعارات المخصصة ل Intune بواسطة تطبيق مدخل الشركة علي جهاز المستخدم.</span><span class="sxs-lookup"><span data-stu-id="804f3-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="804f3-104">ينشئ التطبيق بعد ذلك اعلام الدفع علي ذلك الجهاز.</span><span class="sxs-lookup"><span data-stu-id="804f3-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="804f3-105">فيما يلي المتطلبات الاساسيه للجهاز لدعم إيصال اعلامات مخصصه ، ولكي يقوم التطبيق بإنشاء اعلام الدفع:</span><span class="sxs-lookup"><span data-stu-id="804f3-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="804f3-106">يجب ان يكون تطبيق مدخل الشركة مثبتا علي الجهاز.</span><span class="sxs-lookup"><span data-stu-id="804f3-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="804f3-107">يجب ان يسمح الجهاز لتطبيق مدخل الشركة بإرسال اعلامات الدفع.</span><span class="sxs-lookup"><span data-stu-id="804f3-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="804f3-108">عند تثبيت التطبيق أو تحديثه ، سيطالب المستخدم بالسماح بالاعلامات.</span><span class="sxs-lookup"><span data-stu-id="804f3-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="804f3-109">يجب ان يتم تثبيت خدمات Google Play علي أجهزه Android.</span><span class="sxs-lookup"><span data-stu-id="804f3-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="804f3-110">يجب ان يتم تسجيل الجهاز باستخدام Intune.</span><span class="sxs-lookup"><span data-stu-id="804f3-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="804f3-111">لمزيد من المعلومات ، بما في ذلك كيفيه إرسال رسالة ، راجع [وثائق الميزات](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="804f3-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
