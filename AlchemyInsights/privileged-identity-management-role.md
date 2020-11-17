---
title: دور أداره الهويات المميزة
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
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088484"
---
# <a name="privileged-identity-managementpim-role"></a>دور أداره الهويات المميزة (بيم)

**لا يتم منح الأذونات بعد تنشيط دور**

عند تنشيط دور في أداره الهويات المميزة في Azure AD (بيم) ، قد لا يتم نشر التنشيط فورا إلى كل المداخل التي تتطلب الدور المميز. في بعض الأحيان ، حتى إذا تم نشر التغيير ، فقد يؤدي التخزين المؤقت لويب في المدخل إلى عدم تاثير التغييرات علي الفور.

إذا تم تاجيل التنشيط ، فاتبع الخطوات التالية:

1. تسجيل الخروج من مدخل Azure ثم تسجيل الدخول مجددا. عند تنشيط دور Azure AD أو دور موارد Azure ، ستري مراحل عمليه التنشيط. بمجرد اكتمال كل المراحل ، ستري الارتباط "تسجيل الخروج". يمكنك استخدام هذا الارتباط لتسجيل الخروج. سيؤدي ذلك إلى حل معظم حالات تاخير التنشيط.
2. في بيم ، تاكد من انك قد أدرجت كعضو في الدور.
3. إذا كنت تقوم بتنشيط دور مسؤول Exchange ، فتاكد من تسجيل الخروج وتسجيل الدخول مره أخرى. إذا استمرت المشكلة ، فقم بفتح بطاقة دعم ورفع المشكلة. إذا كنت تستخدم دور مسؤول Exchange للوصول إلى مركز الأمان والتوافق ، فراجع الخطوة التالية.
4. إذا كنت تقوم بتنشيط دور للوصول إلى مركز الأمان والتوافق أو إذا كنت تقوم بتنشيط دور مسؤول SharePoint ، ستواجه بعض التاخير في التنشيط خلال دقائق قليله تصل إلى بضع ساعات. هذه مشكله معروفه ونحن نعمل باستمرار مع هذه الفرق لحل هذه المشكلة بأسرع وقت ممكن.

لمزيد من المعلومات، اطلع على:

- [تنشيط ادوار Azure AD الخاصة بي في بيم](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [تنشيط ادوار موارد Azure في بيم](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**لا تتم أزاله الأذونات بعد إلغاء تنشيط دور أو انتهاء صلاحيه تنشيط الدور**

عند إلغاء تنشيط دور في أداره الهويات المميزة في Azure AD أو عند انتهاء صلاحيه فتره تنشيط دور ، قد يكون هناك تاخير حيث تستمر في الوصول.

إذا تم تاخير إلغاء التنشيط ، فاتبع الخطوات التالية:

1. إذا كنت تقوم بإلغاء تنشيط دور مسؤول Exchange أو إذا انتهت صلاحيه فتره تنشيط الدور ، وظهرت تاخيرا هاما قبل أزاله الأذونات ، فقم بفتح بطاقة دعم وأخبر مهندس الدعم لمساعدتك في الحصول علي البطاقة باستخدام فريق أداره الوصول المسموح به (بأم) داخل Office حول هذه المشكلة.
2. إذا انتهت صلاحيه فتره التنشيط ، ولكنك لا تزال جلسة المستعرض مفتوحة ، فاغلق المستعرض. يمكنك الاستمرار في استخدام الدور حتى تقوم بإغلاق جلسة العمل هذه. هذه مشكله معروفه سنقوم بالاطلاع علي إصلاح محتمل لابطال كل جلسة بشكل فعال عند انتهاء صلاحيه التنشيط.

إذا كانت المهلة الخاصة بك مختلفه عن السيناريوين التاليين ، فالرجاء فتح تذكره دعم.
