---
title: أنواع الاشتراك المدعومة
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
- "9003560"
- "6675"
ms.openlocfilehash: f11eabdc18f708e34a6a10c67bc3e7416330cbf34aec20209b42252ffa0ab018
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072147"
---
# <a name="supported-subscription-types"></a>أنواع الاشتراك المدعومة

يرجى مراجعة أنواع الاشتراك المدعومة للمضي قدمًا.

[أنواع الاشتراك المدعومة](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**نقل ملكية الفواتير**

مدخل Azure كـ [مسؤول الحساب](https://ms.portal.azure.com/) لحساب الفوترة الذي يحتوي على الاشتراك الذي تريد نقله

- ابحث عن **إدارة التكلفة + الفواتير**. حدد **الاشتراكات** من الجزء الأيمن. بناءً على الوصول، قد تحتاج إلى تحديد نطاق فوترة ثم **الاشتراكات** أو **اشتراكات Azure**.
- حدد نقل ملكية الفواتير للاشتراك الذي تريد نقله
- أدخل عنوان البريد الإلكتروني للمستخدم الذي يكون مسؤول الفوترة للحساب الذي سيكون المالك الجديد للاشتراك، ثم حدد **إرسال طلب النقل**
- يتلقى المستخدم رسالة بريد إلكتروني تحتوي على إرشادات لمراجعة طلب النقل الخاص بك. للموافقة على طلب النقل، يختار المستخدم الرابط في البريد الإلكتروني ويتبع التعليمات.

ملاحظة: إذا قمت بنقل ملكية الفوترة لاشتراكك إلى حساب مستخدم في مستأجر Azure AD آخر، فستتم إزالة [جميع تعيينات التحكم في الوصول المستند إلى الدور (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) لإدارة الموارد في الاشتراك بشكل دائم. سيتمكن المالك الجديد فقط من الوصول لإدارة الموارد في الاشتراك. لمزيد من المعلومات، راجع [نقل الاشتراك إلى مستخدم في مستأجر Azure AD آخر](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**نقل ملكية الاشتراك**

يتطلب نقل ملكية الاشتراك أن يفقد الوصول المستند إلى الدور (RBAC) لإدارة الموارد في الاشتراك وصولها. لمزيد من المعلومات حول إضافة اشتراك موجود إلى مستأجر، راجع [اقتران أو إضافة اشتراك Azure إلى Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- لن يتم تحويل الاشتراك بالمبلغ الحالي المستحق من دورة الفوترة الحالية إلى وسيلة الدفع الجديدة في الحساب الجديد. المعلومات الوحيدة المتاحة للمستخدمين في الحساب الجديد هي تكلفة الشهر الماضي لاشتراكك. لا يتم نقل بقية محفوظات الاستخدام والفوترة مع الاشتراك.
- يتم حاليًا دعم نقل ملكية فواتير اشتراكات اتفاقية المؤسسة (EA) في بوابة اتفاقية المؤسسة فقط
- يتطلب تحويل الاشتراك الموجه إلى الائتمان مثل Visual Studio و BizSpark و Microsoft Partner Network إلى مستخدم جديد أن يكون لديه ترخيص شبكة شركاء Visual Studio / Microsoft لقبول طلب النقل
- يتم نقل جميع الموارد مثل الأجهزة الافتراضية والأقراص والمواقع الإلكترونية إلى الحساب الجديد بنجاح. يمكن أن تتأثر الموارد التالية في نقل الاشتراك عبر المستأجرين:

**خدمات مجال Azure AD**

خزائن مفاتيح Azure

- يمكن أن يتأثر [المستخدمون وقواعد البيانات المرتبطة بـ SQL](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support)، خاصةً إذا كان العميل يستخدم مصادقة مرتبطة بـ Azure Active Directory
- قد تتأثر **خدمات التطبيقات** التي تم تكوينها باستخدام مصادقة Azure Active Directory
- قد تفقد حسابات خدمات **Visual Studio Team** المتصلة باشتراكات Azure إمكانية الوصول مؤقتًا عند إلغاء اشتراك Azure المتصل

**المستندات الموصى بها**

خطوات بعد قبول ملكية الفواتير:

- للاحتفاظ بملكية الفوترة، ولكن مع تغيير نوع اشتراكك، راجع: [تبديل اشتراك Azure الخاص بك إلى عرض آخر](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [نقل Visual Studio وشبكة شركاء Microsoft (MPN) ودفع اشتراكات التطوير/الاختبار أثناء السير](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [نقل ملكية الفواتير لاشتراكات اتفاقية المؤسسة (EA)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [الأسئلة الشائعة حول نقل الملكية](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [استكشاف مشكلات نقل الملكية وإصلاحها](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)