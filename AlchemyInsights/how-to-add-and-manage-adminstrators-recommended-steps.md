---
title: كيفيه أضافه المسؤولين وأدارهم-خطوات مستحسنه
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
ms.openlocfilehash: ed3aa5defabdd4f505ee4f74570023d990910dcb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755822"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>كيفيه أضافه المسؤولين وأدارهم-خطوات مستحسنه

بالاستناد إلى وصف المشكلة ، لقد عثرنا علي حل لك. يستطيع معظم العملاء حل مشكلتهم بنفسهم بعد متابعه الوثائق الخاصة بنا.

**تحرير مسؤول الاشتراك أو المسؤول المساعد**

- يمكن لمسؤول الحساب تحرير كل من الأدوار بينما يمكن لمسؤول الاشتراك تغيير المسؤولين المساعدين فقط في [مدخل Azure](https://ms.portal.azure.com/#home).
- [أضافه مسؤولي الاشتراك في Azure أو تغييرهم](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**تحديث مسؤول الاشتراك أو Co-Administrator للاشتراكات الداخلية (أيرس)**

يمكن لمسؤول الخدمة أو المسؤول المساعد المشاركة في هذا الاجراء باستخدام الخطوات التالية:

1. سجل دخولك إلى [مدخل Azure](https://ms.portal.azure.com/#home) وانقر فوق **أداره التكاليف + الفوترة** في الريش اليمني.
2. انقر فوق عنصر البند مع اشتراكك. يؤدي ذلك إلى فتح النظرة العامة حول اشتراكك.
3. علي ريش **الاشتراك** ، انقر فوق **خصائص**. 
4. انقر فوق الزر **مسؤول الخدمة** .
5. ادخل البريد الكتروني الخاص بالمستخدم الذي تريد تعيينه كمسؤول خدمه ، وانقر فوق **موافق**.

**أضافه/تغيير/أزاله المسؤول المساعد**

1. سجل دخولك إلى [مدخل Azure](https://ms.portal.azure.com/#home) كمسؤول خدمه.
2. افتح [الاشتراكات](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) وحدد اشتراكا. (يمكن تعيين الأدمينستراتورس المساعد فقط في نطاق الاشتراك.)
3. الانتقال إلى **التحكم بالوصول (أيام)**  >  **المسؤولون الكلاسيكيون**  >  **أضافه**  >  **أضافه المسؤول المساعد** لفتح الجزء **أضافه** مساعد ، ويشير إلى انه ليس لديك الأذونات).
4. حدد المستخدم الذي تريد اضافته وانقر فوق **أضافه**.

**التعرف على المزيد:**
- [أضافه المسؤول المساعد](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [أزاله المسؤول المساعد](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [تغيير مسؤول الخدمة](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [عرض مسؤول الحساب](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [أداره access باستخدام RBAC و Azure portal](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**أضافه/حذف مستخدمين باستخدام Azure Active directory (AD)**

يمكنك أضافه مستخدمين جدد أو حذف مستخدمين موجودين من مؤسسه Azure Active Directory (Azure AD):

1. لأضافه مستخدم جديد ، سجل دخولك إلى [مدخل Azure](https://ms.portal.azure.com/#home) كمسؤول المستخدم للمؤسسة.
2. حدد **Azure Active** directory ، وحدد **المستخدمون** ، ثم انقر فوق **مستخدم جديد**.
3. في صفحه **المستخدم** ، قم بتعبئة المعلومات المطلوبة. انقر فوق **إنشاء**. يتم إنشاء المستخدم وأضافه إلى مستاجر Azure AD.

**تعرف علي المزيد**:

- [أضافه مستخدم جديد](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [حذف مستخدم](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [أضافه معلومات ملف تعريف المستخدم أو تحديثها باستخدام Azure Active directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**المستندات المستحسنة**

- [ما المقصود بالتحكم في الوصول القائم علي الدور (RBAC) ؟](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [فهم الأدوار المختلفة في Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [أذونات دور المسؤول في Azure Active directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [برنامج تعليمي: منح حق الوصول لمستخدم باستخدام RBAC ومدخل Azure](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [استكشاف أخطاء RBAC وإصلاحها في Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [تنظيم الموارد باستخدام مجموعات أداره Azure](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [كيفيه طلب نسخه من Azure فواتير عبر البريد الكتروني](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [كيفيه أضافه رصيد أو بطاقة سحب أو تحديثها أو ازالتها من Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [أداره اشتراك (أعاده تنشيط/إلغاء الأمر)](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



