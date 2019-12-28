---
title: إرسال اعلامات مخصصه مع اينتوني
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886844"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="55303-102">كيفيه إرسال اعلامات مخصصه لمستخدمي أجهزه iOS و Android المدارة</span><span class="sxs-lookup"><span data-stu-id="55303-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="55303-103">تتم معالجه الاعلامات المخصصة ل اينتوني بواسطة تطبيق "مدخل الشركة" علي جهاز المستخدم.</span><span class="sxs-lookup"><span data-stu-id="55303-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="55303-104">ثم يقوم التطبيق بإنشاء اشعار الدفع علي هذا الجهاز.</span><span class="sxs-lookup"><span data-stu-id="55303-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="55303-105">فيما يلي المتطلبات المسبقة للجهاز لدعم استلام الإشعارات المخصصة ، ولكي يقوم التطبيق بإنشاء اشعار الدفع:</span><span class="sxs-lookup"><span data-stu-id="55303-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="55303-106">يجب ان يكون لدي الجهاز تطبيق "مدخل الشركة" مثبتا.</span><span class="sxs-lookup"><span data-stu-id="55303-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="55303-107">يجب ان يسمح الجهاز لتطبيق بوابه الشركة بإرسال إشعارات الدفع.</span><span class="sxs-lookup"><span data-stu-id="55303-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="55303-108">عند تثبيت التطبيق أو تحديثه ، فانه سيطالب المستخدم بالسماح بالإشعارات.</span><span class="sxs-lookup"><span data-stu-id="55303-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="55303-109">يجب ان يكون لدي أجهزه Android خدمات Google Play مثبته.</span><span class="sxs-lookup"><span data-stu-id="55303-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="55303-110">يجب ان يتم تسجيل الجهاز مع اينتوني.</span><span class="sxs-lookup"><span data-stu-id="55303-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="55303-111">لمزيد من المعلومات بما في ذلك كيفيه إرسال رسالة ، راجع [وثائق الميزة](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="55303-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
