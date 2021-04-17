---
title: نقل ملكية فوترة Azure
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
- "6849"
ms.openlocfilehash: fc02a64807cad61cfeecf04d1f8e38666402583f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820597"
---
# <a name="transfer-azure-billing-ownership"></a>نقل ملكية فوترة Azure

سجّل الدخول إلى [بوابة Azure](https://portal.azure.com/) كمسؤول عن حساب الفوترة الذي يحتوي على الاشتراك الذي تريد نقله. إذا لم تكن متأكدًا مما إذا كنت مسؤولاً، أو إذا كنت بحاجة إلى تحديد من هو المسؤول، فراجع [تحديد مسؤول فوترة الحساب](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

1. ابحث عن _إدارة التكلفة والفوترة_.
1. حدد **الاشتراكات** من الجزء الأيمن. بناءً على الوصول، قد تحتاج إلى تحديد نطاق فوترة ثم **الاشتراكات** أو **اشتراكات Azure**.
1. حدد **نقل ملكية الفواتير** للاشتراك الذي تريد نقله.
1. أدخل عنوان البريد الإلكتروني للمستخدم الذي يلعب دور مسؤول الفوترة للحساب الذي سيكون المالك الجديد للاشتراك، ثم حدد **إرسال طلب النقل**.
1. يتلقى المستخدم رسالة بريد إلكتروني تحتوي على إرشادات لمراجعة طلب النقل الخاص بك. للموافقة على طلب النقل، يختار المستخدم الرابط في البريد الإلكتروني ويتبع التعليمات.

يُرجى ملاحظة أنه إذا قمت بنقل ملكية الفوترة لاشتراكك إلى حساب مستخدم في مستأجر Azure AD آخر، فستتم إزالة جميع تعيينات [التحكم في الوصول المستند إلى الدور (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) لإدارة الموارد في الاشتراك بشكل دائم. سيتمكن المالك الجديد فقط من الوصول لإدارة الموارد في الاشتراك. لمزيد من المعلومات حول كيفية تغيير الدليل للاشتراك، راجع [نقل الاشتراك إلى مستخدم في مستأجر Azure AD آخر](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

_**تأثير مهم على فواتيرك**_: إذا قمت بنقل ملكية الفوترة لاشتراك Azure، فسيتم تقسيم الرسوم الخاصة بك بالتناسب. ستتمكن من الوصول إلى الفواتير وفقًا لما يلي:  

1. حدد اشتراكك من  [صفحة الاشتراكات](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)  في بوابة Azure  [كمستخدم لديه حق الوصول إلى الفواتير](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)، ثم حدد  **الفواتير**.
1. انقر فوق  **تنزيل الفاتورة**  لعرض نسخة من فاتورة PDF الخاصة بك. إذا كانت الرسالة تشير إلى  _غير متوفر_، فراجع  [لماذا لا أرى فاتورة لآخر فترة فوترة؟](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice).
1. يمكنك أيضًا عرض استخدامك اليومي من خلال النقر على **فترة الفوترة** للحصول على ملف PDF لفاتورتك ونسخة من ملف الاستخدام اليومي المفصل (.CSV). لمزيد من المعلومات،  [راجع الحصول على الفاتورة وبيانات الاستخدام](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support).

**المستندات المستحسنة**

- [نقل ملكية الفواتير لاشتراك Azure إلى حساب آخر](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [نبذة عن نقل ملكية الفواتير لاشتراك Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [نقل Visual Studio وشبكة شركاء Microsoft (MPN) ودفع اشتراكات التطوير/الاختبار أثناء السير](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [الأسئلة الشائعة حول نقل الملكية](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [استكشاف مشكلات نقل الملكية وإصلاحها](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
