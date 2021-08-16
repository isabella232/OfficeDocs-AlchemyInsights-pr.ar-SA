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
ms.openlocfilehash: 85cbd89e461f36a51eed816619fd132ea60dfdb0014eb850c7ec3f38d41e1ca2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069951"
---
# <a name="conditional-access-issues"></a>مشاكل الوصول الشرطي

**حل المشاكل المتعلقة ب تشخيص تسجيل الدخول**

يمكنك بسرعة معرفة ما حدث أو تشخيص المشاكل المتعلقة تسجيل الدخول من قبل المستخدم باستخدام [تشخيص تسجيل الدخول:](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. قم ب تشغيل تشخيص تسجيل الدخول.
1. ابحث عن الحدث الذي تريد تحليله بإدخال التفاصيل التي لديك حول المستخدم أو التطبيق أو وقت تسجيل الدخول أو طلب المعرف أو المعرف الارتباطي.
1. راجع النتائج التشخيصية التي تظهر تفاصيل ما حدث والإجراءات التي يمكنك اتخاذها من أجل إجراء تغييرات (إذا كانت هناك حاجة إلى أي تغييرات).

**خطوات استكشاف الأخطاء في تسجيل الدخول وإصلاحها** 

1. انتقل إلى صفحة تسجيل الدخول إلى Azure AD.
1. قم بتصفية تسجيل الدخول حسب المستخدم، النطاق الزمني، التطبيق، الحالة، تطبيق العميل، وما إلى ذلك.
1. حدد حدث تسجيل الدخول وانظر علامة التبويب الوصول الشرطي لمعرفة أي من السياسات تم تقييمها.
1. انقر فوق صف نهج لعرض تفاصيل النهج وفهم سبب تطبيقه.

**أدوات استكشاف الأخطاء في نهج الوصول الشرطي وإصلاحها**

- يسمح لك وضع التقرير فقط بتقييم نهج دون التأثير على المستخدمين.
- تتيح لك أداة ماذا إذا محاكاة أحداث تسجيل الدخول وترى ما هي السياسات التي تنطبق.
- Insights المصنف وإعداد التقارير تأثير الوقت الحقيقي لكل نهج.

**سياسات حماية الأساس**

تم إهمال سياسات حماية الأساس. لم يعد يتم فرضها وستزال قريبا من مدخل Azure. نوصي بتمكين [إعدادات الأمان الافتراضية.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)

لمزيد من المعلومات حول الوصول الشرطي، راجع:

[أفضل الممارسات للوصول الشرطي في Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [الشروط في الوصول الشرطي](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [عناصر التحكم في الوصول الشرطي](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [المواقع في الوصول الشرطي](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
