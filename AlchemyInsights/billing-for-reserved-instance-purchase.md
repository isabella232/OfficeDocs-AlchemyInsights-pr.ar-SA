---
title: الفوترة لشراء مثيل محجوز
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 9d71554d2089a6d9e5d4850149d113959f3d43c0
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820309"
---
# <a name="billing-for-reserved-instance-purchase"></a>الفوترة لشراء مثيل محجوز

يتم محاسبة عملية الشراء المحجوزة على طريقة الدفع المرتبطة بالاشتراك الذي تحدده في وقت الشراء. يجب أن يكون نوع الاشتراك اتفاقية مؤسسة (رقم العرض: MS-AZR-0017P) أو Pay-As-Go (رقم العرض: MS-AZR-0003P) أو اتفاقية عملاء Microsoft أو CSP.

- بالنسبة لاشتراك المؤسسة، يتم خصم الرسوم من رصيد الالتزام النقدي للتسجيل أو يتم خصمها على أنها مبالغ فيها
- بالنسبة إلى اشتراك Pay-As-You-Go، يتم فوترة الرسوم إلى بطاقة الائتمان أو طريقة الدفع بالفاتورة في الاشتراك

**إلغاء الحجز**

- **الخدمة الذاتية:** يمكنك إلغاء مثيل محجوز أو تبادله بنفسك باستخدام [مدخل Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). حدد الحجز وانقر فوق استرداد المبلغ أو التبادل. تجدر الإشارة إلى أنه يجب أن يكون لديك حق وصول المالك في أمر الحجز لتبادل الأموال أو استردادها. لن تسمح لك إمكانية الوصول إلى الحجز فقط بالمتابعة لاسترداد المبلغ أو التبادل. اطلب من مالك أمر الحجز من أن يعطيك حق الوصول إلى أمر الحجز
- **نهج Exchange:** يمكنك تبادل حجز بحجز آخر من النوع نفسه - لا توجد أي **جزاء** على بورصة الحجز. يجب أن يكون إجمالي الالتزام بالحجز الجديد أكبر من مجموع مبلغ استرداد مبلغ الحجز المتبادل والمدفوعات الشهرية المستقبلية (إن أمكن)
- **نهج الاسترداد:** لا يمكن أن يتجاوز مجموع المبالغ المستردة والمدفوعات المستقبلية الملغاة 50000 دولار أمريكي في نافذة ممتدة على 12 شهرا. نحن لا **نطبق حاليا** أي رسوم على المبالغ المستردة ولكن يمكننا فرضها على المبالغ المستردة في المستقبل

**الاستثناءات:** لا تتوفر إمكانية تبادل الخدمة الذاتية والإلغاء لعملاء اتفاقية مؤسسة الحكومة الأمريكية

- **لا يتوفر دعم API / PS / CLI** للإلغاء واسترداد المبالغ المستردة وتبادلات الخدمة الذاتية واسترداد الأموال [لحجوزات Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- لا تتوفر إمكانية تبادل الخدمة الذاتية والإلغاء لعملاء اتفاقية مؤسسة الحكومة الأمريكية. يتم دعم أنواع اشتراكات الحكومة الأمريكية الأخرى بما في ذلك "الدفع عند التنقل" و"CSP"

تعرف على المزيد : [كيفية معالجة](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) معاملات الإرجاع والتبادل تعرف على المزيد : سياسات Exchange [واسترداد](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) الأموال أسئلة أخرى: تفضل بزيارة مستندات [المثيلات المحجوزة](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**تبادل مثيل محجوز موجود (الخدمة الذاتية)**

يمكنك تبادل حجز بحجز آخر من النوع نفسه. يمكنك أيضا استرداد مبلغ حجز يصل إلى 50000 دولار أمريكي في السنة، إذا لم تعد بحاجة إليه. لا تتوفر إمكانية تبادل الخدمة الذاتية والإلغاء لعملاء اتفاقية مؤسسة الحكومة الأمريكية. يتم دعم أنواع اشتراكات حكومية أخرى في الولايات المتحدة بما في ذلك Pay-As-Go و CSP. يجب أن يكون لديك حق وصول المالك في أمر الحجز لتبادل حجز موجود أو استرداد قيمته.

سترشد الخطوات التالية الإجراء الخاص بإكمال المعاملة

1.سجل دخولك إلى مدخل [Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). حدد الحجوزات التي تريد استرداد قيمتها وانقر فوق **Exchange** 2.حدد منتج VM الذي تريد شراءه وا اكتب كمية. تأكد من أن إجمالي الشراء الجديد أكبر من الإجمالي المرجع [تحديد الحجم المناسب قبل الشراء](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3.مراجعة المعاملة وإكمالها

**استرداد المبلغ لمثيل محجوز**

لاسترداد قيمة الحجز، انتقل إلى **تفاصيل الحجز وانقر** فوق **استرداد المبلغ**

**المبلغ المسترد تصنيفا محترفا:**

**أمثلة حول متطلبات الاسترداد** والتبادل مثال الحجز مقدما:

- شراء RI لمدة سنة واحدة بمبلغ 120 ر.سي. في 1 يناير
- في 7 أبريل، تريد استرداد المبلغ أو تبادل هذا الحجز
- نظرا لأن الحجز قد تم لمدة 97 يوما، سوف تحصل على (1-97/365) * 120 دولار للخلف. (أي 88,1 دولار أمريكي). لا توجد حاليا أي عاقبة على المبالغ المستردة
- إذا تبادلت، يجب أن تكون عملية الشراء الجديدة أكبر من 88.1 دولار أمريكي
- لا توجد أي عاقبة على المبالغ المستردة حاليا

**مثال على حجز خطة الفوترة:**

- يمكنك شراء RI لمدة سنة واحدة مقابل 10 دولارات أمريكيه لكل شهر
- في 7 أبريل، تريد استرداد المبلغ أو تبادل هذا الحجز
- بما أن الدفعة الأخيرة قد حدثت خلال 7 أيام، ستحصل على (1-7/31) * $10 للخلف. (أي 7,74 دولار أمريكي)
- المدفوعات المستقبلية الملغاة هي 80 دولارا أمريكيا. لا توجد حاليا أي عاقبة على المبالغ المستردة
- سيتم خصم مبلغ 87.74 دولار من مبلغ الاسترداد الذي تبلغ قيمته 50000 دولار أمريكي
- إذا كانت قيمة التبادل، يجب أن تكون القيمة الإجمالية للشراء الجديد أكبر من 87.74 دولار أمريكي

**تعذر رؤية الفاتورة لفترة الفوترة الأخيرة**

بعض الأسباب المحتملة وراء عدم رؤية فاتورة:

- لديك مبلغ ائتمان شهري مع اشتراكك لم تتجاوزه أو لديك فترة تجريبية مجانية. يتم إنشاء فاتورة فقط عندما تكون مدانا بالمال
- إنه أقل من 30 يوما من اليوم الذي اشتركت فيه في Azure
- لم يتم إنشاء الفاتورة بعد. الانتظار حتى نهاية فترة الفوترة
- إذا لم تكن مسؤول الحساب، فقد لا تكون الفواتير القديمة متوفرة لك

**تنزيل الفاتورة من مدخل Azure (.pdf)**

- حدد اشتراكك من [صفحة](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) الاشتراكات في مدخل Azure كمستخدم [مع إمكانية الوصول إلى الفواتير](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- تحديد **الفواتير**
- انقر **فوق تنزيل الفاتورة** لعرض نسخة من فاتورة PDF. إذا كانت **غير متوفرة**، ف راجع لماذا لا يمكنني رؤية فاتورة لفترة الفوترة [الأخيرة؟](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**تلقي الفاتورة بالبريد الإلكتروني (.pdf)**

- حدد اشتراكك من [صفحة الاشتراكات.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) انقر **فوق الفواتير** ثم أرسل الفاتورة بالبريد الإلكتروني
- انقر **فوق الاشتراك واقبل** الشروط. يجب الاشتراك في كل اشتراك تملكه

ملاحظة: إذا لم تحصل على رسالة بريد إلكتروني بعد اتباع الخطوات، فتأكد من صحة عنوان بريدك الإلكتروني في [تفضيلات](https://account.windowsazure.com/profile) الاتصال على ملف التعريف الخاص بك

**تنزيل بيانات الاستخدام من مدخل Azure**

- تسجيل الدخول إلى [مركز حساب Azure](https://account.windowsazure.com/Subscriptions) [كمسؤول الحساب](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- حدد الاشتراك الذي تريد الحصول على الفاتورة ومعلومات الاستخدام الخاصة به
- حدد **محفوظات الفوترة**
- حدد **عرض البيان الحالي** لرؤية تقدير الرسوم الخاصة بك في الوقت الذي تم فيه إنشاء التقدير
- حدد **تنزيل الاستخدام** لتنزيل بيانات الاستخدام اليومية كملف CSV. إذا رأيت إصدارين متوفرين، ف قم بتنزيل الإصدار 2

أسئلة أخرى: [تفضل بزيارة مستندات المثيلات المحجوزة](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**المستندات المستحسنة**

- [أساسيات الفوترة](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [فهم كيفية تطبيق خصم المثيل المحجوز](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [تنزيل فاتورة فوترة Azure وبيانات الاستخدام اليومية أو عرضها](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [فهم كيفية تطبيق خصم المثيل المحجوز](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [فهم استخدام المثيلات المحجوزة لاشتراكك في Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [فهم استخدام المثيلات المحجوزة للتسجيل في المؤسسة](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [تكاليف برامج Windows غير مضمنة مع المثيلات المحجوزة](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [المثيلات المحجوزة في برنامج Partner Central Cloud Solution Provider (CSP)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)