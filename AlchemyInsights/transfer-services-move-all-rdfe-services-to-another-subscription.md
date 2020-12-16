---
title: نقل الخدمات-نقل كل خدمات ردفي إلى اشتراك آخر
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
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2020
ms.locfileid: "49691915"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>نقل الخدمات-نقل كل خدمات ردفي إلى اشتراك آخر

**نقل الموارد**

يمكن نقل موارد azure إلى اشتراك آخر في Azure أو مجموعه موارد ضمن الاشتراك نفسه باستخدام Azure portal أو Azure PowerShell أو Azure CLI أو REST API لنقل الموارد.

قبل ان تتمكن من نقل الموارد ، راجع:

- [قائمه الاختيار قبل نقل الموارد](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [الخدمات التي يمكن نقلها](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [كيفيه التحقق من صحة النقل](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [نقل إرشادات للخدمات](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

لنقل الموارد الموجودة إلى مجموعه موارد أو اشتراك آخر ، يمكنك استخدام:

- [مدخل Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [واجهه برمجه تطبيقات REST](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

برنامج تعليمي: [نقل موارد Azure إلى مجموعه موارد أخرى أو اشتراك](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**استكشاف الأخطاء وإصلاحها باستخدام Azure Resource Manager**

ارجع إلى المقالات أدناه للتعرف علي بعض أخطاء نشر Azure الشائعة وتلقي معلومات لحلها. إذا لم تتمكن من العثور علي رمز الخطا الخاص برسالة خطا النشر ، فراجع [البحث عن رمز الخطا](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [استكشاف أخطاء النشر وإصلاحها](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [استكشاف أخطاء نقل موارد Azure إلى مجموعه موارد جديده أو الاشتراك فيها](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

لاحظ انه إذا كنت ترغب في ترقيه اشتراكك في Azure ، مثل التبديل من التحديث المجاني إلى الدفع اثناء التنقل ، ستحتاج إلى تحويل اشتراكك.

- لترقيه فتره تجريبية مجانية ، راجع [ترقيه الإصدار التجريبي المجاني أو الاشتراك الخاص ب Microsoft تصور Azure للدفع بالدفع](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- لتغيير حساب الدفع اثناء التنقل ، اطلع علي [تغيير الاشتراك المدفوع باستخدام Azure إلى عرض مختلف](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)عنه.

**لأضافه اشتراك Azure إلى المستاجر الخاص بك في Azure Active Directory أو اقرانه:**

1. سجل الدخول وحدد الاشتراك الذي تريد استخدامه من [صفحه الاشتراكات في مدخل Azure](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).
2. حدد **تغيير الدليل**.
3. راجع اي تحذيرات تظهر ، ثم حدد **تغيير**.
4. يتم تغيير الدليل للاشتراك ستحصل علي رسالة نجاح.
5. استخدم مبدل *الدلائل* للانتقال إلى الدليل الجديد. قد يستغرق عرض كل شيء بشكل صحيح حتى 10 دقائق.

**المستندات المستحسنة**

- [نقل ملكيه اشتراك Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [نقل الموارد إلى مجموعه موارد جديده أو اشتراك](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [أداره الموارد باستخدام مدخل Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
