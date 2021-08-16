---
title: السجلات وإعداد التقارير
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
- "9004331"
- "7727"
ms.openlocfilehash: 03d77c17622a1aac5ecb035bb5b73efdbbfe5e6b141e6b266eef8783f612c8b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54066999"
---
# <a name="logs-and-reporting"></a>السجلات وإعداد التقارير

تجيب الأسئلة الشائعة حول إعداد تقارير [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) على الأسئلة الشائعة حول إعداد تقارير Azure Active Directory (Azure AD). لمزيد من المعلومات، راجع [إعداد تقارير Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).

**استكشاف المشاكل المتعلقة بالمراجعة وإصلاحها**

1. إذا كنت تواجه مشاكل في رؤية بعض أنشطة التدقيق وكان النشاط المفقود في [هذه](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities)القائمة، فيرجى تقديم تذكرة دعم.
2. إذا كنت تواجه مشاكل في رؤية أي سجلات تدقيق في المستأجر، فيرجى تقديم تذكرة دعم.
3. إذا لم تظهر أنشطة التدقيق مباشرة في مدخل Azure، فافحص معلومات زمن الوصول لدينا وأدخل تذكرة دعم إذا تجاوز التأخير زمن زمن الوصول الموثق. [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies)
4. [استبقاء سجلات نشاط Azure AD](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. إذا لم تتمكن من رؤية كل التدقيق لنطاق التاريخ الذي حددته، يمكنك تنزيل ما يصل إلى 250 ألف صف (تم فرزها حسب أحدث الفرز) من مدخل Azure. لمزيد من المعلومات، راجع [تنزيل أنشطة التدقيق](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).

**استكشاف مشاكل تسجيل الدخول وإصلاحها**

1. يمكنك فقط رؤية آخر 30 يوما من البيانات إذا كان لديك ترخيص Azure AD Premium (P1 أو P2) للمستأجر.
2. تتوفر تسجيلات الدخول فقط لمستأجري Azure AD Premium المستأجرين. وهي غير متوفرة للمستأجرين المرخصين المجانيين أو الأساسيين.
3. إذا كان المستأجر لديك Premium P1 ولم تتمكن من رؤية تسجيلات الدخول، [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) فافحص معلومات زمن الوصول لدينا وألف تذكرة دعم إذا تجاوز التأخير زمن الوصول الموثق.
4. إذا لم تتمكن من رؤية كل تسجيلات الدخول لنطاق التاريخ الذي حددته، فلاحظ أنه يمكنك تنزيل ما يصل إلى 250 ألف صف (تم فرزها حسب أحدث الفرز) من مدخل Azure. لمزيد من المعلومات، راجع [تنزيل أنشطة تسجيل الدخول](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).

**استكشاف الأخطاء في تقارير الأمان وإصلاحها (المستخدمون الذين تم وضع علامة على "معرضون للمخاطر"، و"تسجيل الدخول المجازف")**

1. [المستخدمون الذين تم وضع علامة "تقرير أمان المخاطر" لديهم](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [تقرير تسجيل الدخول الخطر في مدخل Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [أحداث المخاطر في Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
