---
title: مشاكل الوصول الشرطي
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014706"
---
# <a name="conditional-access-issues"></a>مشاكل الوصول الشرطي

**حل المشاكل المتعلقة بتشخيص تسجيل الدخول**

يمكنك التعرف بسرعة علي المشاكل المتعلقة بتسجيل الدخول إلى المستخدم باستخدام " [تشخيص تسجيل الدخول](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)":

1. شغل تشخيص تسجيل الدخول.
1. ابحث عن الحدث المراد تحليله عن طريق إدخال التفاصيل التي لديك بشان المستخدم أو التطبيق أو وقت تسجيل الدخول أو معرف الطلب أو معرف الارتباط.
1. راجع نتائج التشخيص التي تعرض تفاصيل ما حدث والإجراءات التي يمكنك اتخاذها لاجراء التغييرات (إذا كانت هناك حاجه إلى التغييرات).

**خطوات استكشاف أخطاء تسجيل الدخول وإصلاحها** 

1. انتقل إلى صفحه تسجيل الدخول إلى Azure AD.
1. تصفيه التسجيلات بواسطة المستخدم والنطاق الزمني والتطبيق والحالة وتطبيق العميل وما إلى ذلك.
1. حدد حدث تسجيل الدخول واعرض علامة تبويب Access الشرطية للاطلاع علي النهج التي تم تقييمها.
1. انقر فوق صف النهج لعرض تفاصيل النهج وفهم سبب التطبيق.

**أدوات لاستكشاف أخطاء نهج Access الشرطي وإصلاحها**

- يتيح لك وضع التقرير فقط تقييم نهج من دون التاثير علي المستخدمين.
- أداه "ماذا إذا" تسمح لك بمحاكاة احداث تسجيل الدخول ومعرفه النهج التي تنطبق.
- تعرض المعارف الدقيقة ومصنف التقارير تاثير الوقت الحقيقي لكل نهج.

**نهج حماية الأساس**

تم إهمال نهج حماية الأساس. لم يعد يتم فرضها ستتم ازالتها قريبا من مدخل Azure. نوصي بتمكين [إعدادات الأمان الافتراضية](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).

للحصول علي مزيد من المعلومات حول الوصول الشرطي ، راجع:

[أفضل الممارسات للوصول الشرطي في Azure Active](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 directory [الشروط في الوصول](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 الشرطي [عناصر التحكم في Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 الشرطي [المواقع في Access الشرطي](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
