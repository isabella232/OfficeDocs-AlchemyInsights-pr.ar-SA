---
title: الفوترة لعمليه شراء مثيل محجوز
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 6cdcb5af27a475cc838eb434ff025eb18356360c
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/30/2020
ms.locfileid: "48822989"
---
# <a name="billing-for-reserved-instance-purchase"></a>الفوترة لعمليه شراء مثيل محجوز

يتحمل شراء المثيل المحجوز طريقه الدفع المرتبطة بالاشتراك الذي تحدده في وقت الشراء. يجب ان يكون نوع الاشتراك اتفاقيه للمؤسسات (رقم العرض: MS-عاذر-0017P) ، الدفع بالعرض الذي ستتم به (الرقم المقدم: MS-عاذر-0003P) أو اتفاقيه عملاء Microsoft أو CSP.

- بالنسبة إلى اشتراك المؤسسة ، يتم خصم الرسوم من رصيد التزام النقدي أو التكلفة التي تفرضها أوفيراجي
- بالنسبة إلى الاشتراك المدفوع بالدفع ، يتم فوتره الرسوم إلى طريقه الدفع الخاصة ببطاقة الائتمان أو الفاتورة في الاشتراك

**إلغاء الحجز**

- **الخدمة الذاتية:** يمكنك إلغاء مثيل محجوز أو exchange بنفسك باستخدام [مدخل Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). حدد الحجز وانقر فوق الاسترداد أو الصرف. لاحظ انه يجب ان يكون لديك حق الوصول إلى المالك في أمر الحجز للتبادل أو الاسترداد. لن يسمح لك الوصول إلى الحجز الا بمتابعه الاسترداد أو الصرف. أسال مالك طلب الحجز بمنحك حق الوصول إلى طلب الحجز
- **نهج Exchange:** يمكنك تبادل حجز لحجز آخر من النوع نفسه-لا توجد **عقوبات** عند حجز exchange. يجب ان يكون إجمالي التزام بالحجز الجديد أكبر من مجموع قيمه المبلغ المسترد للحجز الذي تم تبادله والمدفوعات الشهرية المستقبلية (إذا كان ذلك ممكنا)
- **سياسة الاسترداد:** لا يمكن ان يتجاوز مجموع المبالغ المدفوعة والتي تم إلغاؤها المستقبلية $50,000 دولار في نافذه التداول لمده 12 شهرا. لا نقوم **حاليا بشحن اي جزاءات** في المبالغ المستردة ، ولكنه قد يفرض عليها المبالغ المستردة المستقبلية

**الاستثناءات:** لا تتوفر الميزات الذاتية لتبادل الخدمة وإلغاء لعملاء اتفاقيه المؤسسات الحكومية الامريكيه

- لا يتوفر دعم **واجهه برمجه التطبيق (API)/PS/CLI** لعمليات إلغاء والاسترداد [الذاتي لعمليات الحجز والاسترداد المبالغ المستردة لحجوزات Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- لا تتوفر امكانيه تبادل الخدمة الذاتية وإلغاء لعملاء اتفاقيه المؤسسات الحكومية الامريكيه. أنواع اشتراكات الولايات المتحدة الامريكيه ، بما في ذلك الدفع بالمثل و CSP معتمده

تعرف علي المزيد: [كيفيه معالجه المعاملات الخاصة بالمرتجعات والتبادل تعرف علي المزيد](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) : الاسئله [الأخرى في سياسات Exchange و الاسترداد](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) : [زيارة مستندات المثيل المحجوزة](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Exchange مثيل محجوز موجود (خدمه ذاتية)**

يمكنك تبادل حجز لحجز آخر من النوع نفسه. يمكنك أيضا استرداد مبلغ حجز حتى $50,000 دولار لكل عام ، إذا لم تعد بحاجه اليه. لا تتوفر امكانيه تبادل الخدمة الذاتية وإلغاء لعملاء اتفاقيه المؤسسات الحكومية الامريكيه. أنواع اشتراكات الولايات المتحدة الامريكيه ، بما في ذلك الدفع بالمثل و CSP معتمدين. يجب ان يتوفر لديك حق الوصول إلى المالك في أمر الحجز لتبادل الحجز الحالي أو استرداده.

سترشدك الخطوات التالية علي الاجراء لإكمال المعاملة

1) سجل دخولك إلى [مدخل Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). حدد الحجوزات التي تريد استردادها وانقر فوق **Exchange** 2. حدد منتج VM الذي تريد شراءه واكتب كميه. تاكد من ان إجمالي الشراء الجديد أكبر من العدد الإجمالي الذي [يحدد الحجم الصحيح قبل الشراء](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3. مراجعه المعاملة وإكمالها

**استرداد مثيل محجوز**

لاسترداد قيمه حجز ، انتقل إلى **تفاصيل الحجز** وانقر فوق **المبلغ المسترد**

**المبلغ المسترد ل Pro:**

**أمثله علي نسبه والحد الأدنى لمتطلبات المبالغ لاسترداد الأموال والتبادل** مثال لحجز توجد:

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

**تعذر عرض الفاتورة لفتره الفوترة الاخيره**

بعض الأسباب المحتملة التي قد لا تظهر فيها فاتورة:

- لديك مبلغ رصيد شهري مع اشتراكك الذي لم يتجاوزه أو لديك فتره تجريبية مجانية. يتم إنشاء فاتورة فقط عندما أو مالا
- انها اقل من 30 يوما من اليوم الذي اشتركت فيه في Azure
- لم يتم إنشاء الفاتورة حتى الآن. الانتظار حتى نهاية فتره تحرير الفواتير
- إذا لم تكن مسؤول الحساب ، فقد لا تكون الفواتير القديمة متوفرة لك

**تنزيل فاتورة من Azure portal (.pdf)**

- تحديد اشتراكك من صفحه [الاشتراكات](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) في مدخل Azure [كمستخدم له حق الوصول إلى الفواتير](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- تحديد **الفواتير**
- انقر فوق **تنزيل الفاتورة** لعرض نسخه من فاتورة PDF الخاصة بك. إذا لم يكن الأمر **متوفرا** ، فراجع [لماذا لا يمكنني رؤية فاتورة لفتره الفوترة الاخيره ؟](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**استلام الفاتورة في البريد الكتروني (.pdf)**

- حدد اشتراكك من صفحه " [الاشتراكات](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) ". انقر فوق **الفواتير** ثم إرسال الفاتورة بالبريد الكتروني
- انقر فوق **الموافقة** واقبل الشروط. سيتعين عليك الاشتراك في كل اشتراك تملكه

ملاحظه: إذا لم تحصل علي بريد الكتروني بعد تنفيذ الخطوات ، فتاكد من ان عنوان البريد الكتروني الخاص بك صحيح في [تفضيلات الاتصالات في ملف التعريف الخاص بك](https://account.windowsazure.com/profile)

**تنزيل بيانات الاستخدام من مدخل Azure**

- تسجيل الدخول إلى [مركز حسابات Azure](https://account.windowsazure.com/Subscriptions) [كمسؤول الحساب](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- حدد الاشتراك الذي تريد الحصول علي معلومات الفاتورة والاستخدام الخاصة به
- تحديد **محفوظات الفوترة**
- حدد **عرض الجملة الحالية** للاطلاع علي تقدير للتكاليف في الوقت الذي تم فيه إنشاء التقدير
- حدد **تنزيل الاستخدام** لتنزيل بيانات الاستخدام اليومية كملف CSV. إذا رايت إصدارين متوفرين ، فيمكنك تنزيل الإصدار 2

الاسئله الأخرى: [زيارة مستندات المثيل المحجوزة](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**المستندات المستحسنة**

- [أساسيات الفوترة](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [فهم كيفيه تطبيق خصم المثيل المحجوز](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [تنزيل فاتورة فوتره Azure وبيانات الاستخدام اليومية أو عرضها](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [فهم كيفيه تطبيق خصم المثيل المحجوز](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [فهم استخدام المثيل المحجوز لاشتراك الدفع اثناء التنقل](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [فهم استخدام مثيل محجوز لتسجيل المؤسسة](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [تكاليف برامج Windows غير المضمنة مع المثيلات المحفوظة](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [المثيلات المحفوظة في برنامج موفر حلول السحابة المركزية (CSP) الخاص بالشركاء](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)