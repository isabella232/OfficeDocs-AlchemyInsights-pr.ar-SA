---
title: إدارة الهويات المتميزة الدور
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
ms.openlocfilehash: 358e446192e6b58ace81afa06e0d65ae3a207282351ffc3ec9975a24779951fb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973216"
---
# <a name="privileged-identity-managementpim-role"></a>إدارة الهويات المتميزة (PIM)

**لا يتم منح الأذونات بعد تنشيط دور**

عند تنشيط دور في Azure AD إدارة الهويات المتميزة (PIM)، قد لا يتم نشر التنشيط على الفور على كل المداخل التي تتطلب الدور المميز. في بعض الأحيان، حتى لو تم نشر التغيير، قد يؤدي التخزين المؤقت على الويب في مدخل إلى عدم تطبيق التغيير على الفور.

إذا كان التنشيط متأخرا، فاتبع الخطوات التالية:

1. سجل الخروج من مدخل Azure ثم سجل الدخول مرة أخرى. عند تنشيط دور Azure AD أو دور مورد Azure، سترى مراحل التنشيط. بمجرد اكتمال كل المراحل، سترى ارتباط 'تسجيل الخروج'. يمكنك استخدام هذا الارتباط في تسجيل الخروج. سيحل هذا معظم حالات تأخير التنشيط.
2. في PIM، تحقق من إدراجك كعضو في الدور.
3. إذا كنت تقوم بتنشيط دور المسؤول Exchange، فتأكد من تسجيل الخروج ثم تسجيل الدخول مرة أخرى. إذا استمرت المشكلة، فافتح تذكرة دعم واطرحها كمشكلة. إذا كنت تستخدم دور المسؤول Exchange للوصول إلى مركز التوافق والأمان، فشاهد الخطوة التالية.
4. إذا كنت تقوم بتنشيط دور للوصول إلى مركز الأمان والتوافق أو إذا كنت تقوم بتنشيط دور مسؤول SharePoint، ستختبر بعض تأخير التنشيط من بضع دقائق إلى بضع ساعات. هذه مشكلة معروفة ونعمل بجد مع هذه الفرق لحل هذه المشكلة في أسرع وقت ممكن.

لمزيد من المعلومات، اطلع على:

- [تنشيط أدوار Azure AD في PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [تنشيط أدوار موارد Azure في PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**لا تتم إزالة الأذونات بعد إلغاء تنشيط دور أو انتهاء صلاحية تنشيط الدور**

عند إلغاء تنشيط دور في Azure AD إدارة الهويات المتميزة أو عند انتهاء صلاحية فترة تنشيط الدور، قد يحدث تأخير حيث لا يزال لديك حق الوصول.

إذا تم تأخير إلغاء تنشيطك، فاتبع الخطوات التالية:

1. إذا كنت تقوم بتعطيل دور مسؤول Exchange أو انتهاء فترة تنشيط الدور، ولاحظ وجود تأخير كبير قبل إزالة الأذونات، فافتح تذكرة دعم وأخبر مهندس الدعم لمساعدتك في تقديم تذكرة باستخدام فريق إدارة الوصول المتميز (PAM) داخل Office حول هذه المشكلة.
2. إذا انتهت صلاحية فترة التنشيط، ولكن لا تزال جلسة عمل المستعرض مفتوحة، فاغلق المستعرض. يمكنك الاستمرار في استخدام الدور حتى إغلاق جلسة العمل هذه. هذه مشكلة معروفة وننظر في تصحيح محتمل لإلغاء كل جلسة عمل بشكل نشط بمجرد انتهاء صلاحية التنشيط.

إذا كان تأخيرك مختلفا عن هذين السيناريون، فيرجى فتح تذكرة دعم.
