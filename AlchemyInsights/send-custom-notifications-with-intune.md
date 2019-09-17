---
title: إرسال إعلامات مخصصة باستخدام إينتوني
ms.author: brenduns
author: brenduns
manager: dougeby
ms.date: 07/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000679
ms.openlocfilehash: 1244f07fd56cf603280f1710520a04d579224e44
ms.sourcegitcommit: 16f08d051afca3c6d0de32826324f91cf63ab5ba
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992300"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="44578-102">كيفية إرسال الإخطارات المخصصة لمستخدمي أجهزة دائرة الرقابة الداخلية والروبوت المدارة</span><span class="sxs-lookup"><span data-stu-id="44578-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="44578-103">تتم معالجة الإشعارات المخصصة لـ Intune بواسطة تطبيق بوابة الشركة على جهاز المستخدم.</span><span class="sxs-lookup"><span data-stu-id="44578-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="44578-104">التطبيق ثم يخلق إعلام دفع على هذا الجهاز.</span><span class="sxs-lookup"><span data-stu-id="44578-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="44578-105">فيما يلي المتطلبات المسبقة للجهاز لدعم استلام الإشعارات المخصصة، والتطبيق ثم إنشاء إعلام الدفع:</span><span class="sxs-lookup"><span data-stu-id="44578-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="44578-106">يجب أن يكون الجهاز مثبتًا على تطبيق بوابة الشركة.</span><span class="sxs-lookup"><span data-stu-id="44578-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="44578-107">يجب أن يسمح الجهاز لتطبيق بوابة الشركة بإرسال إشعارات الدفع.</span><span class="sxs-lookup"><span data-stu-id="44578-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="44578-108">عند تثبيت التطبيق أو تحديثه، فإنه سيطالب المستخدم بالسماح بالإشعارات.</span><span class="sxs-lookup"><span data-stu-id="44578-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="44578-109">يجب أن يكون لدى أجهزة Android خدمات Google Play مثبتة.</span><span class="sxs-lookup"><span data-stu-id="44578-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="44578-110">يجب تسجيل الجهاز مع إينتوني.</span><span class="sxs-lookup"><span data-stu-id="44578-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="44578-111">لمزيد من المعلومات بما في ذلك كيفية إرسال رسالة، راجع [وثائق الميزة](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="44578-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
