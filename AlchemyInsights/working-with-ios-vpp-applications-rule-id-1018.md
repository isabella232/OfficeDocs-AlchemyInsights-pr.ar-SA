---
title: العمل باستخدام معرف قاعده تطبيقات iOS فب 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688933"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="e9fb7-102">استخدام تطبيقات iOS فب</span><span class="sxs-lookup"><span data-stu-id="e9fb7-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="e9fb7-103">أقرا [كيفيه أداره تطبيقات iOS التي تم شراؤها من خلال برنامج لشراء وحده التخزين باستخدام Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) للتعرف علي الميزات والقيود والخطوات المتعلقة باستخدام برنامج الشراء الخاص بوحدات التخزين التي تستخدمها والدعم لها في Microsoft intune.</span><span class="sxs-lookup"><span data-stu-id="e9fb7-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="e9fb7-104">**المشاكل الشائعة:** "لقد قمت بتعيين تطبيق iOS فب للمستخدمين ، ولكن فشل التثبيت."</span><span class="sxs-lookup"><span data-stu-id="e9fb7-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="e9fb7-105">قد يحدث هذا في حاله استخدام رمز مميز لفب واحده علي العديد من موفري أداره الاجهزه المحمولة.</span><span class="sxs-lookup"><span data-stu-id="e9fb7-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="e9fb7-106">يمكن استخدام الرموز المميزة لفب من Apple فقط مع موفر واحد.</span><span class="sxs-lookup"><span data-stu-id="e9fb7-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="e9fb7-107">إذا استخدمت رمزا مميزا لفب مع عده موفرين ، فيجب أعاده تحميل الرمز المميز إلى Intune.</span><span class="sxs-lookup"><span data-stu-id="e9fb7-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="e9fb7-108">يمكن ان يفشل التثبيت أيضا إذا تجاوز عدد التثبيتات الإجمالي عدد التراخيص.</span><span class="sxs-lookup"><span data-stu-id="e9fb7-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="e9fb7-109">لعرض تقرير استخدام للتراخيص ، انتقل إلى صفحه تراخيص تطبيق **تطبيقات الاجهزه المحمولة في Intune** \> **App licenses** .</span><span class="sxs-lookup"><span data-stu-id="e9fb7-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="e9fb7-110">لمعرفه كيفيه استرداد التراخيص المستخدمة ، راجع [هذه المقالة.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="e9fb7-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
