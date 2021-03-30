---
title: تطبيق المصادقة
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404187"
---
# <a name="authentication-app"></a>تطبيق المصادقة

إذا كنت المسؤول العام، يمكنك بسرعة معرفة ما حدث أو تشخيص المشاكل المتعلقة تسجيل الدخول من قبل المستخدم باستخدام تشخيص تسجيل [الدخول](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).

1. ابدأ التشخيص بالنقر فوق الزر["تشغيل التشخيص".](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom) 
1. ابحث عن الحدث الذي تريد تحليله بإدخال التفاصيل التي لديك حول المستخدم أو التطبيق أو وقت تسجيل الدخول أو طلب المعرف أو المعرف الارتباطي.
1. راجع نتائج التشخيص التي تظهر تفاصيل ما حدث والإجراءات التي يمكنك اتخاذها من أجل إجراء تغييرات، إذا كانت هناك حاجة إلى أي تغييرات.

**تحقق من السيناريو الذي ينطبق:**

1. إذا لم يحصل المستخدم على إعلام في تطبيق Microsoft Authenticator، فتحقق من عدم إظهاره ضمن المستخدمين المحظورين ل MFA كما هو موضح في حظر المستخدمين و إلغاء [حظرهم.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)
1. إذا لم يتم حظر المستخدم ل MFA ولكنه لم يتلق إعلاما، يمكنه فتح تطبيق Microsoft Authenticator، الذي سيسحب طلبات الموافقة المعلقة.
1. كطريقة بديلة تسجيل الدخول، يمكن للمستخدم أيضا النقر فوق تسجيل الدخول بطريقة أخرى واختيار استخدام رمز التحقق من صحة من تطبيق الأجهزة المحمولة.
1. تطبيق Microsoft Authenticator هو الأسلوب الوحيد المتوفر للعديد من المستخدمين. [تعرف على المزيد حول إعدادات الأمان الافتراضية](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)، تحقق من الأسئلة الشائعة حول الأسئلة الشائعة حول تطبيق [المصادقة](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) وكيفية حلها.
 
**مقاطع الفيديو المستحسنة**

[كيفية إعداد تطبيق Authenticator على هاتف جديد (2 دقيقة)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).
