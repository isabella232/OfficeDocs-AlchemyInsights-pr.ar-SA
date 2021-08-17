---
title: ما يجب فعله إذا لم تعمل ميزات Azure بشكل صحيح في Microsoft Edge
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
ms.openlocfilehash: e188ecb375f3d84b45a1a7718b3c0b797c756f822ba64b3824976fe79c1e8298
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54117075"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>ما يجب فعله إذا لم تعمل ميزات Azure بشكل صحيح في Microsoft Edge

Microsoft Edge مشاكل [معروفة](https://go.microsoft.com/fwlink/?linkid=2140608) مرتبطة بمناطق الأمان وقد تؤثر على كيفية تسجيل مستخدمي Azure الدخول Windows مركز الإدارة. إذا كنت تواجه مشكلة في استخدام ميزات Azure مع Microsoft Edge، فجرب الخطوات التالية:

1. في قائمة **البدء،** ابحث عن **خيارات الإنترنت** وحددها.
2. في مربع **الحوار** خصائص الإنترنت، انتقل إلى علامة **التبويب الأمان.**
3. حدد منطقة **المواقع الموثوق** بها، ثم حدد **الزر مواقع.**
4. في مربع الحوار مواقع **موثوق** بها، أضف عنوان URL البوابة و [https://login.microsoftonline.com](https://login.microsoftonline.com) و ، ثم حدد [https://login.live.com](https://login.live.com) **إغلاق**.
5. في مربع **الحوار** خصائص الإنترنت، انتقل إلى علامة **التبويب الخصوصية.**
6. في المقطع **حظر منبثق،** **حدد** الإعدادات . في مربع الحوار الذي يتم فتحه، أضف عنوان URL البوابة بالإضافة إلى [https://login.microsoftonline.com](https://login.microsoftonline.com) و ، ثم حدد [https://login.live.com](https://login.live.com) **إغلاق**.
