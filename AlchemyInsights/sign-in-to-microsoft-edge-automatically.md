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
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/08/2020
ms.locfileid: "49676705"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>تسجيل الدخول إلى Microsoft Edge تلقائيا

يستخدم Microsoft Edge حساب نظام التشغيل الافتراضي لتسجيل الدخول تلقائيا إلى المستخدم وفقا لكيفيه تكوين جهاز المستخدم. 

يتم وصف سيناريوهات كل نوع من أنواع تكوين الاجهزه وعمليه تسجيل الدخول التابعة له للمستخدم أدناه:

1. **الجهاز مختلط/AAD-J**: يتوفر هذا الخيار علي نظام التشغيل windows 10 والمستوي الأدنى لنظام التشغيل windows وإصدارات خوادم مقابله. يقوم المستخدمون بتسجيل الدخول تلقائيا باستخدام حسابات Azure Active directory (AD) الخاصة بهم.
2. **الجهاز مرتبط بالمجال**: يتوفر هذا الخيار علي نظام التشغيل windows 10 والمستوي الأدنى لنظام التشغيل windows وإصدارات خوادم مقابله. بشكل افتراضي ، لا يتم تسجيل دخول المستخدمين الذين لديهم حسابات المجالات تلقائيا ؛ لتمكين تسجيل الدخول التلقائي لهم ، استخدم نهج **كونفيجوريونبريميسيساككونتاوتوسيجنين** . لتمكين تسجيل الدخول التلقائي للمستخدمين الذين لديهم حسابات Azure AD ، خذ في الاعتبار الانضمام المختلط إلى أجهزتهم.
3. **الحساب الافتراضي لنظام التشغيل هو حساب Microsoft**: يتوفر هذا الخيار علي WINDOWS 10 RS3 (الإصدار 1709 والإنشاء 10.0.16299) والإصدارات الأحدث. هذا السيناريو من المحتمل حدوثه علي أجهزه المؤسسة. ومع ذلك ، إذا كان الحساب الافتراضي لنظام التشغيل هو حساب Microsoft ، سيقوم Microsoft Edge تلقائيا بتسجيل الدخول إلى المستخدم باستخدام حساب Microsoft.
 
 
