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
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398716"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>تسجيل الدخول إلى Microsoft Edge تلقائيا

يستخدم Microsoft Edge الحساب الافتراضي ل OS تسجيل الدخول إلى المستخدم تلقائيا وفقا لكيفية تكوين جهاز المستخدم. 

يتم وصف سيناريوهات كل نوع من أنواع تكوين الجهاز وعملية تسجيل الدخول التابعة للمستخدم أدناه:

- **الجهاز مختلط/AAD-J**: يتوفر هذا الخيار على Windows 10، و Windows بمستوى أدنى، والإصدارات المقابلة من الخادم. يتم تسجيل الدخول تلقائيا إلى المستخدمين باستخدام حسابات Azure Active Directory (AD).
- **الجهاز منضم إلى** المجال : يتوفر هذا الخيار على Windows 10، و Windows بمستوى أدنى، والإصدارات المقابلة من الخادم. بشكل افتراضي، لا يتم تسجيل الدخول تلقائيا إلى المستخدمين الذين لديهم حسابات مجالات؛ لتمكين تسجيل الدخول التلقائي لهم، استخدم النهج **ConfigureOnPremisesAccountAutoSignIn.** لتمكين تسجيل الدخول التلقائي للمستخدمين الذين لديهم حسابات Azure AD، يمكنك الانضمام المختلط إلى أجهزتهم.
- **الحساب الافتراضي لنظام** التشغيل هو حساب Microsoft : يتوفر هذا الخيار على Windows 10 RS3 (الإصدار 1709، النسخة 10.0.16299) والإصدارات الأحدث. من غير المحتمل أن يحدث السيناريو على أجهزة المؤسسة. ومع ذلك، إذا كان حساب نظام التشغيل الافتراضي هو حساب Microsoft، فإن Microsoft Edge سي سجل الدخول تلقائيا إلى المستخدم باستخدام حساب Microsoft.
 
 
