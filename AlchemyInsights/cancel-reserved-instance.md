---
title: إلغاء الحجز
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
- "9003552"
- "6817"
ms.openlocfilehash: 8d0a6a37a244e817472c3949109481a30d80328b7353806905e05c547e196ea0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931220"
---
# <a name="cancelling-reservation"></a>إلغاء الحجز

- **الخدمة الذاتية:** يمكنك إلغاء مثيل محجوز أو استبداله بنفسك باستخدام [مدخل Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). حدد الحجز وانقر على استرداد أو استبدال. لاحظ أنه يجب أن يكون لديك حق وصول المالك في أمر الحجز للاستبدال أو استرداد الأموال. لن يسمح لك الوصول إلى الحجز فقط بمتابعة استرداد الأموال أو استبدالها. اطلب من مالك أمر الحجز أن يمنحك حق الوصول إلى أمر الحجز
- **سياسة الاستبدال:** يمكنك استبدال حجز بحجز آخر من نفس النوع - **لا توجد غرامات** على استبدال الحجز. يجب أن يكون إجمالي الالتزام بالحجز الجديد أكبر من مبلغ استرداد مبلغ الحجز المتبادل والمدفوعات الشهرية المستقبلية (إن وجدت)
- **سياسة الاسترداد:** لا يمكن أن يتجاوز مجموع المبالغ المستردة والمدفوعات المستقبلية الملغاة 50000 دولار أمريكي في فترة 12 شهرًا. نحن **لا نفرض حاليًا أي غرامة** على المبالغ المستردة ولكن يمكننا فرضها على المبالغ المستردة في المستقبل  
    **الاستثناءات:** إمكانية التبادل وإلغاء الخدمة الذاتية غير متوفرة لعملاء اتفاقية المؤسسة الحكومية الأمريكية
- **لا يتوفر دعم API / PS / CLI** للإلغاء واسترداد [عمليات تبادل الخدمة الذاتية والمبالغ المستردة لحجوزات Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- لا تتوفر إمكانية التبادل وإلغاء الخدمة الذاتية لعملاء اتفاقية المؤسسة الحكومية الأمريكية. يتم دعم أنواع اشتراك حكومة الولايات المتحدة الأخرى بما في ذلك Pay-As-You-Go وموفر حلول الحوسبة السحابية من Microsoft

تعرف على المزيد: [كيف تتم معالجة معاملات الإرجاع والاستبدال](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
تعرف على المزيد: [Exchange واسترداد المبلغ المدفوع](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
أسئلة أخرى: [قم بزيارة مستندات المثيل المحجوزة](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Exchange مثيل محجوز موجود (الخدمة الذاتية)**

يمكنك استبدال حجز بحجز آخر من نفس النوع. يمكنك أيضًا استرداد مبلغ الحجز، حتى 50000 دولار أمريكي سنويًا، إذا لم تعد بحاجة إليه. لا تتوفر إمكانية التبادل وإلغاء الخدمة الذاتية لعملاء اتفاقية المؤسسة الحكومية الأمريكية. يتم دعم أنواع اشتراك حكومة الولايات المتحدة الأخرى بما في ذلك Pay-As-You-Go وCSP. يجب أن يكون لديك حق وصول المالك في أمر الحجز لاستبدال أو استرداد حجز موجود.

ستوجه الخطوات التالية كيفية إتمام المعاملة

1. سجل دخولك إلى [مدخل Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). حدد الحجوزات التي تريد استرداد قيمتها وانقر فوق **Exchange**
2. حدد منتج VM الذي تريد شراءه واكتب الكمية. تأكد من أن إجمالي الشراء الجديد أكبر من إجمالي العائد [تحديد الحجم الصحيح قبل الشراء](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. مراجعة المعاملة وإتمامها

**المبالغ المستردة لمثيل محجوز**

لاسترداد مبلغ حجز، انتقل إلى **تفاصيل الحجز** وانقر فوق **استرداد**

**استرداد مقسَّم بالنسب:**

**أمثلة على الاسترداد المقسَّم بالنسب والحد الأدنى من المتطلبات للاسترداد والتبادل**  
مثال حجز مسبق:

- قمت بشراء RI لمدة عام واحد مقابل 120 دولارًا في 1 يناير
- في السابع من أبريل، تريد استرداد أو استبدال هذا الحجز
- نظرًا لأن الحجز ساري المفعول لمدة 97 يومًا، فستحصل على (1-97 / 365) * استرداد 120 دولارًا. (أي 88.1 دولارًا). لا يوجد حاليا أي غرامة على المبالغ المستردة
- في حالة التبادل، يجب أن تكون مشترياتك الجديدة أكبر من 88.1 دولارًا
- لا توجد عقوبة على المبالغ المستردة حاليا

**مثال على حجز خطة الفواتير:**

- تشتري RI لمدة عام واحد مقابل 10 دولارات شهريًا
- في السابع من أبريل، تريد استرداد أو استبدال هذا الحجز
- نظرًا لأن الدفعة الأخيرة حدثت 7 أيام، فستسترد (1-7 / 31) * 10 دولارات أمريكية. (أي 7.74 دولارًا).
- المدفوعات المستقبلية الملغاة 80 دولارًا. لا يوجد حاليا أي غرامة على المبالغ المستردة
- سيؤدي هذا الإلغاء إلى خصم 87.74 دولارًا أمريكيًا من الحد الأقصى لاسترداد المبلغ الذي يبلغ 50000 دولار أمريكي
- في حالة التبادل، يجب أن تكون القيمة الإجمالية للشراء الجديد أكبر من $ 87.74

**المستندات الموصى بها**

- [كيف تتم معالجة معاملات الإرجاع والاستبدال](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [سياسات الاستبدال والاسترداد](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)