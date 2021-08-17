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
ms.openlocfilehash: 4e069a1c75caabf3bef7387140edd5650cf966856b888b5c6b5618a603986d6d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050681"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>تسجيل الدخول إلى Microsoft Edge تلقائيا

Microsoft Edge المستخدم حساب نظام التشغيل الافتراضي لكي يقوم تلقائيا تسجيل الدخول إلى مستخدم وفقا لكيفية تكوين جهاز المستخدم. 

يتم وصف سيناريوهات كل نوع من أنواع تكوين الجهاز وعملية تسجيل الدخول التابعة للمستخدم أدناه:

- **الجهاز مختلط/AAD-J**: يتوفر هذا الخيار على Windows 10 الإصدارات Windows والإصدارات المقابلة للخادم. يتم تسجيل الدخول تلقائيا إلى المستخدمين باستخدام حسابات Azure Active Directory (AD).
- **الجهاز منضم** إلى المجال : يتوفر هذا الخيار على Windows 10 ومستويات Windows والإصدارات المطابقة للخادم. بشكل افتراضي، لا يتم تسجيل الدخول تلقائيا إلى المستخدمين الذين لديهم حسابات مجالات؛ لتمكين تسجيل الدخول التلقائي لهم، استخدم النهج **ConfigureOnPremisesAccountAutoSignIn.** لتمكين تسجيل الدخول التلقائي للمستخدمين الذين لديهم حسابات Azure AD، يمكنك الانضمام المختلط إلى أجهزتهم.
- **حساب نظام التشغيل** الافتراضي هو حساب Microsoft : يتوفر هذا الخيار على Windows 10 RS3 (الإصدار 1709، النسخة 10.0.16299) والإصدارات الأحدث. من غير المحتمل أن يحدث السيناريو على أجهزة المؤسسة. ومع ذلك، إذا كان حساب نظام التشغيل الافتراضي هو حساب Microsoft، Microsoft Edge تسجيل الدخول تلقائيا إلى المستخدم باستخدام حساب Microsoft.
 
 
