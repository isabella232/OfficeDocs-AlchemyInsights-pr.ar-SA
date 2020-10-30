---
title: أنواع الاشتراكات المعتمدة
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6675"
ms.openlocfilehash: 46bc60435c3f8477e9f274d90c39d0f1c6a523c6
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807177"
---
# <a name="supported-subscription-types"></a>أنواع الاشتراكات المعتمدة

يرجى مراجعه أنواع الاشتراكات المعتمدة لمتابعه المزيد.

[أنواع الاشتراكات المعتمدة](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**نقل ملكيه الفوترة**

مدخل Azure [كمسؤول الحساب](https://ms.portal.azure.com/) لحساب الفوترة الذي يحتوي علي الاشتراك الذي تريد نقله

- البحث في **أداره التكاليف + الفوترة** . حدد **الاشتراكات** من الجزء الأيسر. استنادا إلى access ، قد تحتاج إلى تحديد نطاق تحرير فواتير **والاشتراكات** أو **اشتراكات Azure** .
- تحديد نقل ملكيه الفوترة للاشتراك الذي تريد نقله
- ادخل عنوان البريد الكتروني للمستخدم الذي يكون مسؤول الفوترة الخاص بالحساب الذي سيكون مالكه الجديد للاشتراك ، ثم حدد **إرسال طلب تحويل**
- يحصل المستخدم علي رسالة بريد الكتروني تتضمن إرشادات لمراجعه طلب النقل. للموافقة علي طلب النقل ، يقوم المستخدم بتحديد الارتباط في البريد الكتروني واتباع الإرشادات.

ملاحظه: إذا قمت بنقل ملكيه الفوترة لاشتراكك إلى حساب مستخدم في مستاجر Azure AD آخر ، ستتم أزاله كافة تعيينات [التحكم بالوصول المستند إلى الدور (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) لأداره الموارد في الاشتراك بشكل دائم. سيتمكن المالك الجديد فقط من الوصول إلى أداره الموارد في الاشتراك. لمزيد من المعلومات ، راجع [نقل الاشتراك إلى مستخدم في مستاجر AZURE AD آخر](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**نقل ملكيه الاشتراك**

متطلبات الوصول المعتمدة علي الأدوار الخاصة بنقل ملكيه الاشتراك (RBAC) لأداره الموارد في الاشتراك تفقد امكانيه الوصول الخاصة بهم. للحصول علي مزيد من المعلومات حول أضافه اشتراك حالي إلى المستاجر ، راجع [اقران اشتراك azure أو اضافته إلى Azure Active](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support)directory.

- لن يتم نقل تحويل الاشتراك مع مبلغ مستحق حاليا من دوره الفوترة الحالية إلى مستند الدفع الجديد في الحساب الجديد. المعلومات الوحيدة المتوفرة للمستخدمين في حساب جديد هي تكلفه الشهر الماضي لاشتراكك. لا يتم نقل الأجزاء المتبقية من محفوظات الاستخدام والفوترة مع الاشتراك.
- نقل ملكيه الفوترة لاشتراكات اتفاقيه المؤسسة (EA) المعتمدة حاليا في مدخل اتفاقيه المؤسسة فقط
- يمكنك تحويل اشتراك موجه إلى الرصيد مثل Visual Studio و بيزسبارك وشبكه شركاء Microsoft إلى مستخدم جديد لكي تتمكن من الحصول علي ترخيص شبكه شركاء Visual Studio/Microsoft لقبول طلب النقل
- يتم نقل كل الموارد مثل الاجهزه الظاهرية والأقراص ومواقع الويب إلى الحساب الجديد بنجاح. قد تتاثر الموارد التالية في نقل اشتراكات عبر المستاجرين:

**خدمات مجالات Azure AD**

Azure Key فاولتس

- قد يتاثر [المستخدمون وقواعد البيانات المرتبطة ب SQL](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) ، خاصه إذا كان العميل يستخدم مصادقه ذات صله بخدمه Azure Active directory
- قد تتاثر **خدمات التطبيقات** التي تم تكوينها باستخدام مصادقه Azure active directory
- **فريق Visual Studio** قد تفقد حسابات الخدمات المتصلة باشتراكات Azure وصولا مؤقتا عند إلغاء اشتراك Azure المتصل

**المستندات المستحسنة**

خطوات بعد قبول ملكيه الفوترة:

- للاحتفاظ بملكيه الفوترة ، ولكن قم بتغيير نوع الاشتراك الخاص بك ، وأشر [إلى: تبديل اشتراكك في Azure إلى عرض آخر](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [نقل الرسومات في Visual Studio وشبكه شركاء Microsoft (مبن) والدفع بالاضافه إلى الشركات المطورة/التجريبية](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [نقل ملكيه الفوترة لاشتراكات اتفاقيه المؤسسة (EA)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [نقل الاسئله المتداولة حول الملكية](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [استكشاف مشاكل تحويل الملكية وإصلاحها](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)