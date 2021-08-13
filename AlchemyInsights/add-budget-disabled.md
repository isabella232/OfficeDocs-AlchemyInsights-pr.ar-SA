---
title: لماذا تم تعطيل الزر إضافة موازنة لي؟
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
- "9003547"
- "6464"
ms.openlocfilehash: 1263662184948ed1e77e3abacd17babf4aa033ed1ecec29b4c4afc26d6da56f0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53954648"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>لماذا تم تعطيل الزر إضافة موازنة لي؟

لإنشاء موازنة، تحتاج إلى أحد الأذونات التالية:

- مجموعة الإدارة، الاشتراك، نطاقات مجموعة الموارد
- المساهم في إدارة التكاليف
- المالك
- المساهم
- عميل المؤسسة فقط: التسجيل والقسم ونطاقات الحسابات
- مسؤول التسجيل (تعيين الموازنة في نطاق التسجيل)
- مسؤول القسم (تعيين الموازنة في نطاق القسم)
- مالك الحساب (تعيين الموازنة في نطاق الحساب)
- اتفاقية العملاء الحديثة فقط: حساب الفوترة، ملف تعريف الفوترة، نطاقات قسم الفاتورة
- منشئ اشتراك Azure

**لقد أنشأت موازنة عندما كانت تكلفة الشهر الحالي أكثر من الميزانية. لماذا لم أتلق تنبيها؟**  
إذا تجاوزت بالفعل حد تكلفة معين عند إنشاء موازنة لن يتم فيها إطلاق التنبيه. بمجرد بدء دورة جديدة، إذا قمت بخرق العتبة، سيتم بدء التنبيه.

**متى يجب أن أتوق لتلقي تنبيه بعد أن أتجاوز إحدى عتبات تنبيه الموازنة المحددة؟**  
يتم تقييم الموازنات كل 4 ساعات. يستغرق وصول بيانات الاستخدام إلى نظام الموازنات ما لا يقل عن 8 ساعات. على هذا النحو، قد تستغرق التنبيهات 12 ساعة للانطلاق بعد تجاوز الحد.

**لماذا يتم تعطيل زر تاريخ البدء عند تحديد فترة إعادة تعيين شهر أو فوترة؟**  
يتم محاذاة الميزانيات مع شهر التقويم الحالي أو فترة الفوترة الحالية (في حالة تحديد شهر الفوترة). لذلك، نقوم ب ملء هذه القيمة مسبقا لك.

**لماذا لا يمكنني رؤية رسم بياني للتكاليف في تجربة إنشاء الموازنة؟**  
نحتاج إلى بيانات التكلفة لمدة شهرين كحد أدنى قبل أن يمكننا عرض رسم بياني لمساعدتك في إنشاء الموازنة.

**لماذا لا يمكنني تعيين موازنة مقابل اشتراك أنشأته للتو؟**  
بعد إنشاء اشتراك، تستغرق معالجة البيانات من 24 إلى 48 ساعة قبل تعيين موازنة مقابلها.

**موارد API للموازنة**

- [الموازنات API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): يوفر عمليات لإنشاء الموازنات وتحديثها. باستخدام API الموازنات، يمكنك تعيين حد الموازنة وتكوين تنبيهات متعددة للانطلاق عند الاقتراب من هذه العتبة. يمكن أن تقوم التنبيهات بتشغيل رسالة بريد إلكتروني أو مجموعة إجراءات Azure لتنفيذ التنفيذ التلقائي. ملاحظة: لا تتوافق التصفية ل API هذه مع تصفية /أبعاد API للاستعلام.
- [الموازنات API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): إنشاء ميزانيات بقدرات تصفية تكلفة أكبر من v1. تمت محاذاة التصفية إلى العقد المستخدم في واجهات برمجة التطبيقات للاستعلامات والأبعاد. هذه هي برمجة (API) الميزانيات الموصى بها لاستخدام الانتقال إلى الأمام.
- [الأبعاد](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): يوفر عمليات للحصول على أبعاد مدعمة لاستخدامك ضمن مجموعة متنوعة من النطاقات. باستخدام API الأبعاد، يمكنك استرداد قائمة الأبعاد التي يمكن استخدامها كمدخلات إنشاء الاستعلامات باستخدام API للاستعلام.
- [الاستعلام:](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support)يوفر عمليات للحصول على بيانات التكلفة والاستخدام المجمعة استنادا إلى الاستعلام الذي توفره. باستخدام API للاستعلام، يمكنك تحديد التصفية والفرز والت تجميع المطلوب على جميع الأبعاد المتوفرة (التي يتم الوصول إليها من API الأبعاد).

**التكاليف المتوقعة**

**لماذا لا يمكنني رؤية التنبؤات الخاصة بالتكاليف في تحليل التكلفة؟**  
هناك أسباب متعددة وراء فقدان عرض التنبؤ بالنسبة لك في تحليل التكلفة، وبعضها كالتالي:

1. إذا كانت بيانات التكلفة أقل من 10 أيام، لن يتم تحميل مخطط التنبؤ. يتطلب النموذج 10 أيام على الأقل من بيانات التكلفة الأخيرة للحصول على توقعات دقيقة
2. إذا قمت بتحديد تواريخ تاريخية، فإن مخطط التنبؤ لن يكون مرئيا. يرجى تحديد نطاق تاريخ مع تواريخ مستقبلية لمخطط التنبؤ الذي سيتم عرضه
3. إذا كان حسابك به عملات متعددة، فإن مخطط التنبؤ لن يتكبد سوى تكاليف المشروع 'جميع التكاليف بالدولار الأمريكي'

**لماذا لا يتغير التنبؤ عند إجراء تغييرات على مواردي؟**  
يتطلب نموذج التنبؤ بضعة أيام لحساب التغييرات في الحساب ولا يقوم بإجراء توقعات فورية بالاستناد إلى التغيير في الموارد  
للحصول على خطوات أكبر لزيادة الموارد أو إنقاصها، سيستغرق النموذج وقتا أطول قليلا لضبط هذه التغييرات لحساب حالات الشذوذ

**لماذا يزداد التنبؤ بعد الحجز أو شراء السوق؟**  
يأخذ نموذج التنبؤ في الاعتبار "التكلفة الفعلية" ولا يأخذ في الاعتبار الاستخدام والشراء بشكل منفصل. للشراء مرة واحدة، سيخفض النموذج الإسقاطات بعد 10 أيام لحسبان الزيادة المفاجئة في التكاليف

**أريد رؤية التنبؤات لبعد واحد (على سبيل المثال. عداد)**  
تدعم التنبؤات حاليا إجمالي توقعات التكلفة وليس للعدادات الفردية. وبالتالي، عند "تجميع حسب" بعد، ستكون الإسقاطات لإجمالي كل العناصر في البعد

**المستندات الموصى بها**

- [ما هو Azure Cost Management؟](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [أفضل ممارسات إدارة تكاليف Azure](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [تحليل التكاليف والإنفاق](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [استكشاف التكاليف وتحليلها باستخدام تحليل التكلفة](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [إدارة تكاليف Azure: الأسعار](https://azure.microsoft.com/services/cost-management/#pricing)
- [مراجعة التكاليف في تحليل التكلفة](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [فيديو تعليمي: إنشاء موازنة في مدخل Azure](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [المتطلبات الأساسية لعرض الموازنات وتخصيصها](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [إنشاء الميزانيات وإدارتها](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [تكوين التنفيذ التلقائي باستخدام مجموعات إجراءات Azure و API الموازنات](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [استخدام تنبيهات التكلفة لمراقبة الاستخدام والإنفاق](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [أفضل ممارسات إدارة التكاليف](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**مقاطع فيديو تعليمية**

- [إنشاء موازنة في مدخل Azure](https://go.microsoft.com/fwlink/?linkid=2146761)
- [إدارة التكاليف باستخدام API الموازنات ومجموعات الإجراءات](https://go.microsoft.com/fwlink/?linkid=2147038)