---
title: إلغاء الحجز
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
- "9003552"
- "6817"
ms.openlocfilehash: 04875e33f07c6d0a4306b3579ef81f2d28c7f506
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807178"
---
# <a name="cancelling-reservation"></a>إلغاء الحجز

- **الخدمة الذاتية:** يمكنك إلغاء مثيل محجوز أو exchange بنفسك باستخدام [مدخل Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). حدد الحجز وانقر فوق الاسترداد أو الصرف. لاحظ انه يجب ان يكون لديك حق الوصول إلى المالك في أمر الحجز للتبادل أو الاسترداد. لن يسمح لك الوصول إلى الحجز الا بمتابعه الاسترداد أو الصرف. أسال مالك طلب الحجز بمنحك حق الوصول إلى طلب الحجز
- **نهج Exchange:** يمكنك تبادل حجز لحجز آخر من النوع نفسه-لا توجد **عقوبات** عند حجز exchange. يجب ان يكون إجمالي التزام بالحجز الجديد أكبر من مجموع قيمه المبلغ المسترد للحجز الذي تم تبادله والمدفوعات الشهرية المستقبلية (إذا كان ذلك ممكنا)
- **سياسة الاسترداد:** لا يمكن ان يتجاوز مجموع المبالغ المدفوعة والتي تم إلغاؤها المستقبلية $50,000 دولار في نافذه التداول لمده 12 شهرا. لا نقوم **حاليا بشحن اي جزاءات** في المبالغ المستردة ، ولكنه قد يفرض عليها المبالغ المستردة المستقبلية  
    **الاستثناءات:** لا تتوفر الميزات الذاتية لتبادل الخدمة وإلغاء لعملاء اتفاقيه المؤسسات الحكومية الامريكيه
- لا يتوفر دعم **واجهه برمجه التطبيق (API)/PS/CLI** لعمليات إلغاء والاسترداد [الذاتي لعمليات الحجز والاسترداد المبالغ المستردة لحجوزات Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- لا تتوفر امكانيه تبادل الخدمة الذاتية وإلغاء لعملاء اتفاقيه المؤسسات الحكومية الامريكيه. أنواع اشتراكات الولايات المتحدة الامريكيه ، بما في ذلك الدفع بالمثل و CSP معتمده

تعرف علي المزيد: [كيفيه معالجه حركات المرتجعات والتبادل](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
تعرف علي [المزيد: سياسات Exchange و الاسترداد](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
الاسئله الأخرى: [زيارة مستندات المثيل المحجوزة](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Exchange مثيل محجوز موجود (خدمه ذاتية)**

يمكنك تبادل حجز لحجز آخر من النوع نفسه. يمكنك أيضا استرداد مبلغ حجز حتى $50,000 دولار لكل عام ، إذا لم تعد بحاجه اليه. لا تتوفر امكانيه تبادل الخدمة الذاتية وإلغاء لعملاء اتفاقيه المؤسسات الحكومية الامريكيه. أنواع اشتراكات الولايات المتحدة الامريكيه ، بما في ذلك الدفع بالمثل و CSP معتمدين. يجب ان يتوفر لديك حق الوصول إلى المالك في أمر الحجز لتبادل الحجز الحالي أو استرداده.

سترشدك الخطوات التالية علي الاجراء لإكمال المعاملة

1. سجل دخولك إلى [مدخل Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). حدد الحجوزات التي تريد استردادها وانقر فوق **Exchange**
2. حدد منتج VM الذي تريد شراءه واكتب الكمية. تاكد من ان إجمالي الشراء الجديد أكبر من العدد الإجمالي الذي [يحدد الحجم الصحيح قبل الشراء](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. مراجعه المعاملة وإكمالها

**استرداد مثيل محجوز**

لاسترداد قيمه حجز ، انتقل إلى **تفاصيل الحجز** وانقر فوق **المبلغ المسترد**

**المبلغ المسترد ل Pro:**

**أمثله علي نسبه والحد الأدنى لمتطلبات المبالغ لاسترداد الأموال والتبادل**  
مثال لحجز توجد:

- انك تشتري مصطلحا واحدا لمده عاما ل $120 في 1 يناير
- في سابع ، لقد أردت استرداد مبلغ الحجز أو exchange
- نظرا لبقاء الحجز في غضون 97 يوما ، ستحصل علي (1-97/365) * $120 مره أخرى. (علي سبيل المثال $88.1). لا توجد حاليا اي جزاءات في المبالغ المستردة
- إذا قمت بالتبادل ، فيجب ان تكون عمليه الشراء الجديدة أكبر من $88.1
- لا يوجد جزاءات في المبالغ المستردة حاليا

**مثال علي حجز خطه الفوترة:**

- ستشتري مصطلحا واحدا لمده عاما لمده $10 شهريا
- في سابع ، لقد أردت استرداد مبلغ الحجز أو exchange
- منذ المرة الاخيره التي حدثت فيها الدفعة ، ستحصل علي (1-7/31) * $10 مره أخرى. (علي سبيل المثال $7.74)
- المدفوعات المستقبلية التي تم إلغاؤها هي $80. لا توجد حاليا اي جزاءات في المبالغ المستردة
- سيؤدي هذا إلغاء إلى خصم $87.74 من ان الحد الأقصى لمبلغ الاسترداد هو $50,000
- إذا كان الأمر "تبادل" ، فيجب ان تكون القيمة الاجماليه لعمليه الشراء الجديدة أكبر من $87.74

**المستندات المستحسنة**

- [كيفيه معالجه حركات المرتجعات والتبادل](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [سياسات Exchange و الاسترداد](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)