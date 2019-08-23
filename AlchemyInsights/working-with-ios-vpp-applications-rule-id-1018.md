---
title: العمل مع دائرة الرقابة الداخلية 1018 معرف القاعدة تطبيقات الصوت
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: a0bbc1f49f251ef4f16300c8cca98e219008d17e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36557964"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="cf05f-102">العمل مع "تطبيقات الصوت" دائرة الرقابة الداخلية</span><span class="sxs-lookup"><span data-stu-id="cf05f-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="cf05f-103">قراءة [كيفية إدارة تطبيقات دائرة الرقابة الداخلية التي تم شراؤها من خلال برنامج حجم الشراء مع إينتوني Microsoft](https://docs.microsoft.com/intune/vpp-apps-ios) للتعرف على الميزات والقيود وخطوات لجعل استخدام "برنامج شراء حجم التفاح" والدعم له في Microsoft إينتوني.</span><span class="sxs-lookup"><span data-stu-id="cf05f-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="cf05f-104">**المسائل:** "تم تعيينها تطبيق الصوت دائرة الرقابة الداخلية للمستخدمين، ولكن فشل التثبيت."</span><span class="sxs-lookup"><span data-stu-id="cf05f-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="cf05f-105">قد يحدث هذا إذا تم استخدام رمز الصوت واحد عبر عدة موفري إدارة الجهاز المحمول.</span><span class="sxs-lookup"><span data-stu-id="cf05f-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="cf05f-106">يمكن استخدام الرموز المميزة للصوت من التفاح فقط مزود واحد.</span><span class="sxs-lookup"><span data-stu-id="cf05f-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="cf05f-107">إذا استخدمت رمز الصوت مع شركات متعددة، يجب إعادة تحميل الرمز المميز إينتوني.</span><span class="sxs-lookup"><span data-stu-id="cf05f-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="cf05f-108">أيضا يمكن أن تفشل عملية التثبيت في حالة تجاوز العدد الإجمالي لعمليات تثبيت عدد التراخيص.</span><span class="sxs-lookup"><span data-stu-id="cf05f-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="cf05f-109">لعرض تقرير استخدام للتراخيص الخاصة بك، انتقل إلى **التطبيقات المحمولة إينتوني** \> الصفحة **التطبيق التراخيص** .</span><span class="sxs-lookup"><span data-stu-id="cf05f-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="cf05f-110">لمعرفة كيفية استعادة التراخيص في الاستخدام، راجع [هذه المقالة.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="cf05f-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
