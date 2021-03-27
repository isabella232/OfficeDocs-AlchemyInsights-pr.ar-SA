---
title: تسجيل الدخول إلى Microsoft Edge يدويا
ms.author: v-smandalika
author: v-smandalika
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9003844"
- "6893"
- "8332"
- "9004625"
ms.openlocfilehash: f380d09dc14788205638cdee6aebe0b084ecab2f
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398644"
---
# <a name="sign-in-to-microsoft-edge-manually"></a><span data-ttu-id="dd6cd-102">تسجيل الدخول إلى Microsoft Edge يدويا</span><span class="sxs-lookup"><span data-stu-id="dd6cd-102">Sign in to Microsoft Edge manually</span></span>

<span data-ttu-id="dd6cd-103">إذا لم يكن المستخدم قد سجل الدخول تلقائيا أثناء تجربة التشغيل الأولى، يمكن للمستخدم تسجيل الدخول يدويا من خلال إعدادات المستعرض أو قائمة الهوية من قائمة منتحلة.</span><span class="sxs-lookup"><span data-stu-id="dd6cd-103">If a user isn't automatically signed in during a first-run experience, the user can manually sign in through the browser's settings or the identity flyout.</span></span> <span data-ttu-id="dd6cd-104">لإدارة تسجيل الدخول، استخدم السياسات التالية:</span><span class="sxs-lookup"><span data-stu-id="dd6cd-104">To manage sign-in, use the following policies:</span></span>

1. <span data-ttu-id="dd6cd-105">[NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) - للتأكد من أن المستخدم لديه دائما ملف تعريف عمل في Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="dd6cd-105">[NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) - To ensure that a user always has a work profile in Microsoft Edge.</span></span>
2. <span data-ttu-id="dd6cd-106">[RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) - لتقييد تسجيل الدخول إلى مجموعة من الحسابات الموثوق بها.</span><span class="sxs-lookup"><span data-stu-id="dd6cd-106">[RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) - To restrict sign-in to a set of trusted accounts.</span></span>
3. <span data-ttu-id="dd6cd-107">[BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) - لتعطيل تسجيل الدخول أو إجبار المستخدمين على تسجيل الدخول.</span><span class="sxs-lookup"><span data-stu-id="dd6cd-107">[BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) - To disable sign-in or to force users to sign in.</span></span>

