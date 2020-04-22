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
# <a name="working-with-ios-vpp-applications"></a>العمل مع تطبيقات IOS VPP

اقرأ [كيفية إدارة تطبيقات iOS التي تم شراؤها من خلال برنامج شراء وحدة التخزين مع Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) للتعرف على الميزات والقيود والخطوات للاستفادة من برنامج شراء حجم Apple والدعم له في Microsoft Intune.
  
 **القضايا الشائعة:** "لقد عيّن تُعيّن تطبيق IOS VPP للمستخدمين، ولكن التثبيت فشل."
  
- يمكن أن يحدث هذا إذا تم استخدام رمز مميز واحد لـ VPP عبر العديد من موفري إدارة الأجهزة المحمولة. يمكن استخدام رموز VPP من Apple فقط مع مزود واحد. إذا كنت تستخدم رمز ًا مميزًا لـ VPP مع العديد من موفري الخدمة، فيجب عليك إعادة تحميل الرمز المميز إلى Intune.

- يمكن أن يفشل التثبيت أيضًا إذا تجاوز إجمالي عدد عمليات التثبيت عدد التراخيص. لعرض تقرير استخدام لتراخيصك، انتقل إلى صفحة \> **تراخيص** **تطبيقات تطبيقات Intune Mobile.** لمعرفة كيفية استعادة التراخيص في الاستخدام راجع [هذه المقالة.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
