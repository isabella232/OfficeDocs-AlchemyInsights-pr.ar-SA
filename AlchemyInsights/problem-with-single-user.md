---
title: مشكلة مع مستخدم واحد
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: 8d8821cda94b2af244fa317707421f9d197b6052fb316789cd286ea8b4adf19e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960138"
---
# <a name="problem-with-single-user"></a>مشكلة مع مستخدم واحد

- قد لا يتم توفير الخدمة للمستخدم نظرا لعدم فرصة تقييم المستخدم بعد. راجع الإرشادات المتعلقة بمدى الوقت الذي يستغرقه توفير الإعداد بالإضافة إلى شريط التقدم على صفحة تكوين توفير. إذا كانت الحالة المثبت المحددة في مقطع التفاصيل الإضافية قبل تاريخ إنشاء/تحديث/حذف المستخدم، فهذا يعني أننا لم نقيم المستخدم بعد. في هذا السيناريو، أفضل شيء يجب فعله هو انتظار انتهاء خدمة توفير الخدمة.

  - لاحظ أن خدمتنا على علم فقط بالتغييرات التي يتم إدخالها على المستخدم في النظام المصدر (الموارد البشرية في السحابة). يجب أن يكون هناك تغيير صحيح في النظام المصدر ل Azure AD للكشف عن التغيير وتدفقه إلى Active Directory.
- تم تقييم خدمة توفير المستخدم وحدد أنه لا يجب توفيرها:
  - إذا قمت بتعيين عامل تصفية تحديد تحديد حسب السمة، فتأكد من أن المستخدم يلبي المعايير التي حددتها.
  - إذا كان المستخدمون موجودين بالفعل في النظام الهدف وفي حالة المستخدم في تطابق المصدر والهدف، فلن نقوم بأي إجراء آخر.
- حاول توفير الخدمة توفير المستخدم وفشلت. بالنسبة إلى هذه السيناريوهات، راجع علامة التبويب استكشاف الأخطاء وإصلاحها والتوصيات لسجلات توفير الخدمات:
  - قد تكون السمة المطلوبة على المستخدم مفقودة في Active Directory أو Azure AD. على سبيل المثال، لا يتم إنشاء القيمة الصحيحة لقواعد الجيل userPrincipalName أو sAMAccountName.
  - لا يتم حل السمة المطابقة (عادة ما تكون employeeId) لمستخدم فريد في Active Directory المحلي أو Azure AD. على سبيل المثال، هناك مستخدمان لنفس الموظف في AD وترجع الخدمة رمز خطأ يشير إلى إدخالات هدف مكررة لنفس إدخال المصدر.

لمراجعة السجلات لمستخدم واحد ومجموعات واحدة، راجع مراجعة سجلات توفير مشكلة [مع مستخدم معين](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).
