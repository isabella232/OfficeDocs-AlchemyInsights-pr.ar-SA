---
title: نقل ملكيه الفوترة في Azure
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
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/03/2020
ms.locfileid: "48921989"
---
# <a name="transfer-azure-billing-ownership"></a>نقل ملكيه الفوترة في Azure

قم بتسجيل الدخول إلى [مدخل Azure](https://portal.azure.com/) كمسؤول لحساب الفوترة الذي يحتوي علي الاشتراك الذي تريد نقله. إذا لم تكن متاكدا مما إذا كنت أنت والمسؤول ، أو إذا كنت بحاجه إلى تحديد الأشخاص ، فراجع التعرف علي [مسؤول فوتره الحساب](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

- البحث في **أداره التكاليف + الفوترة**.
- حدد **الاشتراكات** من الجزء الأيمن. استنادا إلى access ، قد تحتاج إلى تحديد نطاق تحرير فواتير **والاشتراكات** أو **اشتراكات Azure**.
- تحديد **نقل ملكيه الفوترة** للاشتراك الذي تريد نقله
- ادخل عنوان البريد الكتروني للمستخدم الذي يكون مسؤول الفوترة الخاص بالحساب الذي سيكون مالكه الجديد للاشتراك ، ثم حدد **إرسال طلب تحويل**
- يحصل المستخدم علي رسالة بريد الكتروني تتضمن إرشادات لمراجعه طلب النقل. للموافقة علي طلب النقل ، يقوم المستخدم بتحديد الارتباط في البريد الكتروني واتباع الإرشادات.

**ملاحظه** : إذا قمت بنقل ملكيه الفوترة لاشتراكك إلى حساب مستخدم في مستاجر Azure AD آخر ، ستتم أزاله كافة تعيينات [التحكم بالوصول المستند إلى الدور (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)لأداره الموارد في الاشتراك بشكل دائم. سيتمكن المالك الجديد فقط من الوصول إلى أداره الموارد في الاشتراك. لمزيد من المعلومات ، راجع [نقل الاشتراك إلى مستخدم في مستاجر AZURE AD آخر](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**المستندات المستحسنة**

- [نقل ملكيه الفوترة لاشتراك Azure إلى حساب آخر](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [حول تحويل ملكيه الفوترة لاشتراك Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [نقل الرسومات في Visual Studio وشبكه شركاء Microsoft (مبن) والدفع بالاضافه إلى الشركات المطورة/التجريبية](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [نقل الاسئله المتداولة حول الملكية](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [استكشاف مشاكل تحويل الملكية وإصلاحها](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
