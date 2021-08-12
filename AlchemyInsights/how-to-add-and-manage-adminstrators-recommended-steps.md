---
title: كيفية إضافة المسؤولين وإدارتهم - الخطوات الموصى بها
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 5aa6f11d31ed62078fdd05090af5722289544c5ab2244a369182f4e0f9214183
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963774"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>كيفية إضافة المسؤولين وإدارتهم - الخطوات الموصى بها

استنادا إلى وصف المشكلة، لقد عثرنا على حل لك. تمكن معظم العملاء من حل المشكلة الخاصة بهم بمفردهم بعد متابعة وثائقنا.

**تحرير مسؤول الاشتراك أو المسؤول المشترك**

- يمكن لمسؤول الحساب تحرير كلا الدورين بينما يمكن لمسؤول الاشتراك تغيير المسؤولين ال معاونين فقط في [مدخل Azure](https://ms.portal.azure.com/#home).
- [إضافة مسؤولي اشتراك Azure أو تغييرهم](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**تحديث مسؤول الاشتراك أو Co-Administrator الداخلي (AIRS)**

يمكن لمسؤول الخدمة أو المسؤول المشترك القيام بهذا الإجراء ذاتيا باستخدام الخطوات التالية:

1. سجل دخولك إلى [مدخل Azure وانقر](https://ms.portal.azure.com/#home) فوق **إدارة التكلفة + الفوترة** في النصل الأيمن.
2. انقر فوق عنصر السطر مع اشتراكك. يفتح ذلك نظرة عامة على اشتراكك.
3. على شفرة **الاشتراك،** انقر فوق **خصائص**. 
4. انقر فوق **الزر مسؤول** الخدمة.
5. أدخل البريد الإلكتروني للمستخدم الذي تريد تعيينه كمسؤول خدمة وانقر فوق **موافق.**

**إضافة/تغيير/إزالة المسؤول المشترك**

1. سجل دخولك إلى [مدخل Azure](https://ms.portal.azure.com/#home) كمسؤول خدمة.
2. افتح [الاشتراكات](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) وحدد اشتراكا. (يمكن تعيين المسؤولين المشتركين فقط في نطاق الاشتراك.)
3. انتقل إلى التحكم في **Access (IAM)** المسؤولون التقليديون إضافة مسؤول معاون لفتح الجزء إضافة مسؤول معاون (إذا كان الخيار إضافة مسؤول معاون معطلا، فإنه يشير إلى أنك لا تملك  >    >    >   الأذونات). 
4. حدد المستخدم الذي تريد إضافته وانقر فوق **إضافة**.

**التعرف على المزيد:**
- [إضافة "مسؤول"](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [إزالة مسؤول زميل](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [تغيير مسؤول الخدمة](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [عرض مسؤول الحساب](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [إدارة الوصول باستخدام مدخل RBAC و Azure](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**إضافة/حذف مستخدمين باستخدام Azure Active Directory (AD)**

يمكنك إضافة مستخدمين جدد أو حذف مستخدمين موجودين من مؤسسة Azure Active Directory (Azure AD):

1. لإضافة مستخدم جديد، سجل دخولك إلى مدخل [Azure](https://ms.portal.azure.com/#home) كمسؤول مستخدم في المؤسسة.
2. حدد **Azure Active Directory**، وحدد **المستخدمون** ثم انقر فوق **مستخدم جديد**.
3. في صفحة **المستخدم،** قم بتعبئة المعلومات المطلوبة. انقر **فوق إنشاء**. يتم إنشاء المستخدم وإضافته إلى مستأجر Azure AD.

**تعرف على المزيد:**

- [إضافة مستخدم جديد](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [حذف مستخدم](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [إضافة معلومات ملف تعريف مستخدم أو تحديثها باستخدام Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**المستندات المستحسنة**

- [ما هو عنصر التحكم بالوصول المستند إلى الدور (RBAC)؟](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [فهم الأدوار المختلفة في Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [أذونات دور المسؤول في Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [البرنامج التعليمي: منح حق الوصول لمستخدم يستخدم RBAC ومدخل Azure](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [استكشاف الأخطاء في RBAC في Azure وإصلاحها](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [تنظيم الموارد باستخدام مجموعات إدارة Azure](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [كيفية طلب نسخة من فاتورة Azure عبر البريد الإلكتروني](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [كيفية إضافة بطاقة ائتمان أو خصم أو تحديثها أو إزالتها من Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [إدارة (إعادة تنشيط/إلغاء/تبديل) الاشتراك](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



