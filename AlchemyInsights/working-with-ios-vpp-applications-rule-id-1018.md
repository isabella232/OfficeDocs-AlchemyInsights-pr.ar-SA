---
title: العمل مع معرف قاعدة تطبيقات VPP iOS 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719944"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="2b5b0-102">العمل مع تطبيقات IOS VPP</span><span class="sxs-lookup"><span data-stu-id="2b5b0-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="2b5b0-103">اقرأ [كيفية إدارة تطبيقات iOS التي تم شراؤها من خلال برنامج شراء وحدة التخزين مع Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) للتعرف على الميزات والقيود والخطوات للاستفادة من برنامج شراء حجم Apple والدعم له في Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="2b5b0-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="2b5b0-104">**القضايا الشائعة:** "لقد عيّن تُعيّن تطبيق IOS VPP للمستخدمين، ولكن التثبيت فشل."</span><span class="sxs-lookup"><span data-stu-id="2b5b0-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="2b5b0-105">يمكن أن يحدث هذا إذا تم استخدام رمز مميز واحد لـ VPP عبر العديد من موفري إدارة الأجهزة المحمولة.</span><span class="sxs-lookup"><span data-stu-id="2b5b0-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="2b5b0-106">يمكن استخدام رموز VPP من Apple فقط مع مزود واحد.</span><span class="sxs-lookup"><span data-stu-id="2b5b0-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="2b5b0-107">إذا كنت تستخدم رمز ًا مميزًا لـ VPP مع العديد من موفري الخدمة، فيجب عليك إعادة تحميل الرمز المميز إلى Intune.</span><span class="sxs-lookup"><span data-stu-id="2b5b0-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="2b5b0-108">يمكن أن يفشل التثبيت أيضًا إذا تجاوز إجمالي عدد عمليات التثبيت عدد التراخيص.</span><span class="sxs-lookup"><span data-stu-id="2b5b0-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="2b5b0-109">لعرض تقرير استخدام لتراخيصك، انتقل إلى صفحة \> **تراخيص** **تطبيقات تطبيقات Intune Mobile.**</span><span class="sxs-lookup"><span data-stu-id="2b5b0-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="2b5b0-110">لمعرفة كيفية استعادة التراخيص في الاستخدام راجع [هذه المقالة.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="2b5b0-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
