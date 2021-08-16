---
title: MC210173 - إهمال ميزة النموذج المخصص الجديدة في SharePoint Designer
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: f72d6ce6931b39d5d4a4835cee0ed2952407b13187213cca5bd483acb1e192bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54077638"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a>MC210173 - إهمال ميزة النموذج المخصص الجديدة في SharePoint Designer

لقد عرفنا مشكلة تؤثر على وظيفة SharePoint Designer من أجل [إنشاء نماذج مخصصة](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) في SharePoint Online. بعد الفحص الدقيق، قررنا أنه لا يوجد حل معروف لهذه المشكلة واخترنا تعطيل ميزة إنشاء النموذج المخصصة اعتباراً من الساعة 3:00 صباحاً بالتوقيت العالمي المنسق يوم السبت 25 أبريل 2020. لا يؤثر هذا التغيير على إمكانية تحرير النماذج التي تم إنشاؤها مسبقاً أو الميزات الموجودة الأخرى في SharePoint Online Designer.

بعد إجراء هذا التغيير، ربما يكون المستخدمون قد تلقوا الخطأ: "تعذر حفظ تغييرات القائمة على الخادم"، عند إنشاء نماذج جديدة.

وبدلاً من ذلك، يمكن للمستخدمين الذين استفادوا من SharePoint Designer لإنشاء نماذج مخصصة استخدام [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) لهذا الغرض.

PowerApps هي أداة سهلة وفعالة تتيح للمستخدمين الذين يعملون في تجربة SharePoint Online Modern إنشاء نماذج مخصصة وتحريرها لقوائم SharePoint ومكتبات المستندات مباشرة من نافذة المستعرض. لا يتطلب PowerApps معرفة التعليمات البرمجية التقليدية أو أي تنزيلات إضافية للتطبيقات مثل InfoPath.

**ملاحظة**: سيحتاج مستخدمو SharePoint Online Classic إلى التبديل مؤقتاً إلى التجربة الحديثة للوصول إلى PowerApps والاستفادة منها؛ على الرغم من ذلك، يمكن الوصول إلى جميع النماذج المخصصة التي تم إنشاؤها في PowerApps بواسطة مستخدمي تجربة SharePoint Online Classic.
