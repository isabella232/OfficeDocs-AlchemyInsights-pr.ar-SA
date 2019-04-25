---
title: العمل مع دائرة الرقابة الداخلية 1018 معرف القاعدة تطبيقات الصوت
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 65b9a727171a7551068717f6327f15e1aa8e6bed
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420471"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="f4793-102">العمل مع "تطبيقات الصوت" دائرة الرقابة الداخلية</span><span class="sxs-lookup"><span data-stu-id="f4793-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="f4793-103">قراءة [كيفية إدارة تطبيقات دائرة الرقابة الداخلية التي تم شراؤها من خلال برنامج حجم الشراء مع إينتوني Microsoft](https://docs.microsoft.com/intune/vpp-apps-ios) للتعرف على الميزات والقيود وخطوات لجعل استخدام "برنامج شراء حجم التفاح" والدعم له في Microsoft إينتوني.</span><span class="sxs-lookup"><span data-stu-id="f4793-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span> 
  
 <span data-ttu-id="f4793-104">**المسائل:** "تم تعيينها تطبيق الصوت دائرة الرقابة الداخلية للمستخدمين، ولكن فشل التثبيت."</span><span class="sxs-lookup"><span data-stu-id="f4793-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span> 
  
- <span data-ttu-id="f4793-105">قد يحدث هذا إذا تم استخدام رمز الصوت واحد عبر عدة موفري إدارة الجهاز المحمول.</span><span class="sxs-lookup"><span data-stu-id="f4793-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="f4793-106">يمكن استخدام الرموز المميزة للصوت من التفاح فقط مزود واحد.</span><span class="sxs-lookup"><span data-stu-id="f4793-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="f4793-107">إذا استخدمت رمز الصوت مع شركات متعددة، يجب إعادة تحميل الرمز المميز إينتوني.</span><span class="sxs-lookup"><span data-stu-id="f4793-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>
    
- <span data-ttu-id="f4793-108">أيضا يمكن أن تفشل عملية التثبيت في حالة تجاوز العدد الإجمالي لعمليات تثبيت عدد التراخيص.</span><span class="sxs-lookup"><span data-stu-id="f4793-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="f4793-109">لعرض تقرير استخدام للتراخيص الخاصة بك، انتقل إلى **التطبيقات المحمولة إينتوني** \> الصفحة **التطبيق التراخيص** .</span><span class="sxs-lookup"><span data-stu-id="f4793-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="f4793-110">لمعرفة كيفية استعادة التراخيص في الاستخدام، راجع [هذه المقالة.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="f4793-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
    

