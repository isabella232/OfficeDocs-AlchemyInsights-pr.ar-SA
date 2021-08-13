---
title: نقل الخدمات - نقل كل خدمات RDFE إلى اشتراك آخر
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
- "9004116"
- "7196"
ms.openlocfilehash: 89217922b8b51f2548f9fff53bf80364c0e897b1d9b34bfb7016f0b0f197cf17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940015"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>نقل الخدمات - نقل كل خدمات RDFE إلى اشتراك آخر

**نقل الموارد**

يمكن نقل موارد Azure إما إلى اشتراك Azure آخر أو مجموعة موارد ضمن الاشتراك نفسه باستخدام مدخل Azure أو Azure PowerShell أو Azure CLI أو REST API لنقل الموارد.

قبل أن تتمكن من نقل الموارد، راجع:

- [قائمة الاختيار قبل نقل الموارد](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [الخدمات التي يمكن نقلها](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [كيفية التحقق من صحة عملية الانتقال](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [نقل الإرشادات الخاصة بالخدمات](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

لنقل الموارد الموجودة إلى مجموعة موارد أو اشتراك آخر، يمكنك استخدام:

- [مدخل Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

البرنامج التعليمي: [نقل موارد Azure إلى مجموعة موارد أخرى أو اشتراك آخر](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**استكشاف الأخطاء وإصلاحها باستخدام Azure Resource Manager**

راجع المقالات أدناه للتعرف على بعض أخطاء النشر الشائعة في Azure وتلقي معلومات لحلها. إذا لم تتمكن من العثور على رمز الخطأ لخطأ النشر، فشاهد [البحث عن رمز الخطأ](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [استكشاف أخطاء النشر وإصلاحها](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [استكشاف الأخطاء المتعلقة بتحريك موارد Azure إلى مجموعة موارد جديدة أو اشتراك جديد وإصلاحها](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

تجدر الإشارة إلى أنك إذا كنت تريد ترقية اشتراكك في Azure، مثل التبديل من مجاني إلى "الدفع مع التنقل"، ستحتاج إلى تحويل اشتراكك.

- لترقية فترة تجريبية مجانية، راجع ترقية اشتراك الإصدار التجريبي المجاني أو [Microsoft Imagine Azure إلى Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- لتغيير حساب "الدفع مع الانتقال"، راجع تغيير اشتراكك في [Azure Pay-As-You-Go إلى عرض مختلف](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).

**لإضافة اشتراك Azure إلى مستأجر Azure Active Directory أو إقرانه:**

1. سجل الدخول وحدد الاشتراك الذي تريد استخدامه من صفحة الاشتراكات [في مدخل Azure](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).
2. حدد **تغيير الدليل**.
3. راجع أي تحذيرات تظهر، ثم حدد **تغيير**.
4. يتم تغيير الدليل للاشتراك وستحصل على رسالة نجاح.
5. استخدم *مبدل* الدليل للذهاب إلى الدليل الجديد. قد يستغرق إظهار كل شيء بشكل صحيح ما يصل إلى 10 دقائق.

**المستندات الموصى بها**

- [نقل ملكية اشتراك Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [نقل الموارد إلى مجموعة موارد جديدة أو اشتراك جديد](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [إدارة الموارد باستخدام مدخل Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
