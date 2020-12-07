---
title: ما يجب فعله إذا كانت ميزات Azure لا تعمل بشكل صحيح في Microsoft Edge
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583159"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>ما يجب فعله إذا كانت ميزات Azure لا تعمل بشكل صحيح في Microsoft Edge

يتضمن Microsoft Edge [مشاكل معروفه](https://go.microsoft.com/fwlink/?linkid=2140608) تتعلق بمناطق الأمان وقد تؤثر علي كيفيه تسجيل المستخدمين في Azure إلى مركز أداره Windows. إذا كنت تواجه مشكله في استخدام ميزات Azure مع Microsoft Edge ، فجرب الخطوات التالية:

1. في القائمة **بدء** ، ابحث عن **خيارات الإنترنت** وحددها.
2. في مربع الحوار **خصائص إنترنت** ، انتقل إلى علامة التبويب **أمان** .
3. حدد منطقه **المواقع الموثوق بها** ، ثم حدد الزر **مواقع** .
4. في مربع الحوار **مواقع موثوق بها** ، أضف عنوان URL للبوابة بالاضافه إلى [https://login.microsoftonline.com](https://login.microsoftonline.com) ، ثم [https://login.live.com](https://login.live.com) حدد **إغلاق**.
5. في مربع الحوار **خصائص إنترنت** ، انتقل إلى علامة التبويب **الخصوصية** .
6. في المقطع **حظر الإطارات المنبثقة** ، حدد **إعدادات**. في مربع الحوار الذي يتم فتحه ، أضف عنوان URL للبوابة بالاضافه إلى [https://login.microsoftonline.com](https://login.microsoftonline.com) [https://login.live.com](https://login.live.com) ، ثم حدد **إغلاق**.
