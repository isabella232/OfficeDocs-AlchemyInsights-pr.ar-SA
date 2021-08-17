---
title: الفوترة لشراء المثيل المحجوز
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
ms.openlocfilehash: 00565470de388165e64c45879c22fd5064b4adc695151edaf58878f38a481ff2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104007"
---
# <a name="billing-for-reserved-instance-purchase"></a>الفوترة لشراء المثيل المحجوز

يتم تحميل تكلفة شراء المثيل المحجوز على طريقة الدفع المرتبطة بالاشتراك الذي تحدده في وقت الشراء. يجب أن يكون نوع الاشتراك اتفاقية Enterprise (رقم العرض: MS-AZR-0017P)، الاستحقاق أولاً بأول (رقم العرض: MS-AZR-0003P)، اتفاقية عملاء Microsoft أو موفر حلول الحوسبة السحابية من Microsoft (CSP).

- بالنسبة إلى اشتراك المؤسسة، يتم خصم الرسوم من رصيد الالتزام النقدي للقيد، أو احتسابها كفائض.
- بالنسبة لاشتراك الاستحقاق أولاً بأول، تتم فوترة الرسوم على بطاقة الائتمان أو طريقة سداد الفاتورة على الاشتراك

**إلغاء الحجز**

- **الخدمة الذاتية:** يمكنك إلغاء مثيل محجوز أو استبداله بنفسك باستخدام [مدخل Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). حدد الحجز وانقر على استرداد أو استبدال. لاحظ أنه يجب أن يكون لديك حق وصول المالك في أمر الحجز للاستبدال أو استرداد الأموال. لن يسمح لك الوصول إلى الحجز فقط بمتابعة استرداد الأموال أو استبدالها. اطلب من مالك أمر الحجز أن يمنحك حق الوصول إلى أمر الحجز
- **سياسة الاستبدال:** يمكنك استبدال حجز بحجز آخر من نفس النوع - **لا توجد غرامات** على استبدال الحجز. يجب أن يكون إجمالي الالتزام بالحجز الجديد أكبر من مبلغ استرداد مبلغ الحجز المتبادل والمدفوعات الشهرية المستقبلية (إن وجدت)
- **سياسة الاسترداد:** لا يمكن أن يتجاوز مجموع المبالغ المستردة والمدفوعات المستقبلية الملغاة 50000 دولار أمريكي في فترة 12 شهرًا. نحن **لا نفرض حاليًا أي غرامة** على المبالغ المستردة ولكن يمكننا فرضها على المبالغ المستردة في المستقبل

**الاستثناءات:** إمكانية التبادل وإلغاء الخدمة الذاتية غير متوفرة لعملاء اتفاقية المؤسسة الحكومية الأمريكية

- **لا يتوفر دعم API / PS / CLI** للإلغاء واسترداد [عمليات تبادل الخدمة الذاتية والمبالغ المستردة لحجوزات Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- لا تتوفر إمكانية التبادل وإلغاء الخدمة الذاتية لعملاء اتفاقية المؤسسة الحكومية الأمريكية. يتم دعم أنواع اشتراك حكومة الولايات المتحدة الأخرى بما في ذلك Pay-As-You-Go وموفر حلول الحوسبة السحابية من Microsoft

تعرف على المزيد: [كيفية](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) معالجة معاملات الإرجاع والتبادل تعرف على المزيد [:](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) Exchange ونهج الاسترداد أسئلة أخرى: تفضل بزيارة مستندات [المثيلات المحجوزة](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Exchange مثيل محجوز موجود (الخدمة الذاتية)**

يمكنك استبدال حجز بحجز آخر من نفس النوع. يمكنك أيضًا استرداد مبلغ الحجز، حتى 50000 دولار أمريكي سنويًا، إذا لم تعد بحاجة إليه. لا تتوفر إمكانية التبادل وإلغاء الخدمة الذاتية لعملاء اتفاقية المؤسسة الحكومية الأمريكية. يتم دعم أنواع اشتراك حكومة الولايات المتحدة الأخرى بما في ذلك Pay-As-You-Go وCSP. يجب أن يكون لديك حق وصول المالك في أمر الحجز لاستبدال أو استرداد حجز موجود.

ستوجه الخطوات التالية كيفية إتمام المعاملة

1.سجل دخولك إلى مدخل [Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). حدد الحجوزات التي تريد استرداد قيمتها **وانقر** فوق Exchange 2.حدد منتج VM الذي تريد شراءه وا اكتب كمية. تأكد من أن إجمالي الشراء الجديد أكبر من الإجمالي المرجع [تحديد الحجم المناسب قبل الشراء](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3.مراجعة المعاملة وإكمالها

**المبالغ المستردة لمثيل محجوز**

لاسترداد مبلغ حجز، انتقل إلى **تفاصيل الحجز** وانقر فوق **استرداد**

**استرداد مقسَّم بالنسب:**

**Pro على الحد** الأدنى من متطلبات الاسترداد والتبادل مثال الحجز مقدما:

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

**تعذر رؤية الفاتورة لفترة الفوترة الأخيرة**

بعض الأسباب المحتملة وراء عدم رؤية فاتورة:

- لديك مبلغ ائتمان شهري مع اشتراكك لم تتجاوزه أو لديك فترة تجريبية مجانية. يتم إنشاء فاتورة فقط عندما تكون مدانا بالمال
- إنه أقل من 30 يوما من اليوم الذي اشتركت فيه في Azure
- لم يتم إنشاء الفاتورة بعد. الانتظار حتى نهاية فترة الفوترة
- إذا لم تكن مسؤول الحساب، فقد لا تكون الفواتير القديمة متوفرة لك

**تنزيل الفاتورة من مدخل Azure (.pdf)**

- حدد اشتراكك من [صفحة](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) الاشتراكات في مدخل Azure كمستخدم [مع إمكانية الوصول إلى الفواتير](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- تحديد **الفواتير**
- انقر فوق **تنزيل الفاتورة** لعرض نسخة من فاتورة PDF الخاصة بك. إذا كانت الرسالة **غير متوفرة**، فراجع [لماذا لا أرى فاتورة لآخر فترة فوترة؟](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

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

أسئلة أخرى: [قم بزيارة مستندات المثيل المحجوزة](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**المستندات الموصى بها**

- [أساسيات الفوترة](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [فهم كيفية تطبيق خصم المثيل المحجوز](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [تنزيل فاتورة فوترة Azure وبيانات الاستخدام اليومية أو عرضها](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [فهم كيفية تطبيق خصم المثيل المحجوز](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [فهم استخدام المثيلات المحجوزة لاشتراكك في Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [فهم استخدام المثيلات المحجوزة للتسجيل في المؤسسة](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windows البرامج غير المضمنة مع المثيلات المحجوزة](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [المثيلات المحجوزة في برنامج الشريك Cloud Solution Provider (CSP)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)