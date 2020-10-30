---
title: لماذا تم تعطيل زر أضافه موازنة لي ؟
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
- "9003547"
- "6464"
ms.openlocfilehash: 18edad73f617ba180cb08576ee6e5fa8faf07128
ms.sourcegitcommit: 9a7b85eae0bb775bc2498a83d8f5fedb72a6451e
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807153"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>لماذا تم تعطيل زر أضافه موازنة لي ؟

لإنشاء موازنة ، تحتاج إلى أحد الأذونات التالية:

- مجموعه الاداره ، الاشتراك ، نطاقات مجموعات الموارد
- المساهم في أداره التكلفة
- المالك
- مساهم
- عميل علي مستوي المؤسسة فقط: التسجيل والقسم ونطاقات الحسابات
- مسؤول التسجيل (تعيين الموازنة في نطاق التسجيل)
- المسؤول عن القسم (تعيين الموازنة في نطاق القسم)
- مالك الحساب (تعيين الموازنة في نطاق الحساب)
- اتفاقيه عميل حديثه فقط: حساب الفوترة ، ملف تعريف الفوترة ، نطاقات مقطع الفاتورة
- منشئ الاشتراك في Azure

**لقد قمت بإنشاء ميزانيه عندما كانت تكلفه الشهر الحالي تتجاوز الموازنة. لماذا لم أتلقى تنبيه ؟**  
إذا تجاوزت بالفعل عتبه تكلفه معينه عندما تقوم بإنشاء موازنة ، فلن يتم إطلاق التنبيه. بمجرد ان تبدا دوره جديده ، إذا قمت بخرق العتبة ، سيتم إطلاق التنبيه.

**متى يجب ان أتوقع تلقي تنبيه بعد تجاوز أحد عتبات تنبيات الموازنة المعرفة الخاصة بي ؟**  
يتم تقييم الميزانيات كل 4 ساعات. يستغرق الأمر حدا ادني 8 ساعات لاستخدام البيانات للوصول إلى نظام الموازنات. لقد اعطي لك هذا الاجراء ، قد تستغرق التنبيات ما دام 12 ساعة ليتم إطلاقها بعد تجاوز الحد الفاصل.

**لماذا يتم تعطيل زر "تاريخ البدء" عند تحديد فتره أعاده تعيين شهر أو شهر الفوترة ؟**  
تتم محاذاة الموازنات إلى شهر التقويم الحالي أو فتره الفوترة الحالية (في حاله تحديد شهر الفوترة). ولذلك ، قمنا مسبقا بملء هذه القيمة نيابة عنك.

**لماذا لا يمكنني رؤية رسم بياني للتكاليف في تجربه إنشاء الموازنة ؟**  
نحتاج إلى الحد الأدنى لمده 2 شهرا من بيانات التكلفة قبل ان نتمكن من تقديم رسم بياني لمساعدتك في إنشاء الموازنة.

**لماذا لا يمكنني تعيين موازنة مقابل اشتراك قمت بإنشاءه للتو ؟**  
بعد إنشاء الاشتراك ، تستغرق البيانات 24-48 ساعة للمعالجة قبل تعيين موازنة مقابلها.

**موارد واجهه برمجه التطبيق للموازنة**

- [الميزانيات API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): توفر عمليات لإنشاء الموازنات وتحديثها. باستخدام واجهه برمجه التطبيق الخاصة بالموازنات ، يمكنك تعيين عتبه الموازنة وتكوين تنبيات متعددة لتشغيلها باعتبارك الحد الفاصل. بإمكان التنبيات تشغيل رسالة بريد الكتروني أو مجموعه إجراءات Azure لتنفيذ التنفيذ التلقائي. ملاحظه: لا تتم محاذاة التصفية الخاصة بواجهة برمجه التطبيقات هذه مع الابعاد/تصفيه API للاستعلام.
- [الميزانيات API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): إنشاء موازنات باستخدام قدرات تصفيه تكاليف أكبر من v1. يتم محاذاة التصفية إلى العقد المستخدم في واجات برمجه التطبيقات الخاصة بالاستعلام والابعاد. هذه هي الميزانيات الموصي بها لاستخدام API الانتقال إلى الامام.
- [الابعاد](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): توفير العمليات للحصول علي الابعاد المعتمدة لاستخدامك ضمن مجموعه من النطاقات. باستخدام واجهه برمجه تطبيقات الابعاد ، يمكنك استرداد قائمه بالابعاد التي يمكن استخدامها كادخالات لإنشاء الاستعلامات باستخدام واجهه برمجه تطبيقات الاستعلام.
- [استعلام](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): يوفر عمليات للحصول علي بيانات التكلفة المجمعة والاستخدام استنادا إلى الاستعلام الذي توفره. باستخدام API للاستعلام ، يمكنك تحديد التصفية المطلوبة والفرز والتجميع في كل الابعاد المتوفرة (التي يتم الوصول اليها من واجهه برمجه تطبيقات الابعاد).

**التكاليف المتوقعة**

**لماذا لا يمكنني رؤية التنبؤات الخاصة بتكاليفي في تحليل التكلفة ؟**  
ثمة أسباب عديده لأنه قد يكون عرض التنبؤ مفقودا بالنسبة اليك في تحليل التكلفة ، وهي كالتالي:

1. إذا كانت بيانات التكلفة اقل من 10 أيام ، فلن يتم تحميل مخطط التنبؤ. يتطلب النموذج 10 أيام علي الأقل من بيانات التكلفة الاخيره للحصول علي التوقعات الدقيقة
2. إذا قمت بتحديد تواريخ تاريخيه ، فلن يظهر مخطط التنبؤ. يرجى تحديد نطاق تاريخ يحتوي علي تواريخ مستقبليه لعرض المخطط التنبؤ
3. إذا كان حسابك يحتوي علي عده عملات ، سيقوم المخطط التنبؤ فقط بتكاليف ' كل التكاليف بالدولار الأمريكي '

**لماذا لا يتغير التنبؤ عند اجراء تغييرات علي الموارد ؟**  
يتطلب نموذج التنبؤ عددا من الأيام لحساب التغييرات في الحساب ولا يتم اجراء الإسقاطات المباشرة استنادا إلى التغيير في الموارد  
للحصول علي خطوات أكبر لزيادة الموارد أو تقليلها ، سيستغرق النموذج وقتا أطول قليلا لضبط هذه التغييرات علي حساب ل أنوماليس

**لماذا يزداد التنبؤ بعد اجراء حجز أو شراء موقع تسوق ؟**  
يعتبر نموذج التنبؤ "التكلفة الفعلية" ولا يقوم بحساب الاستخدام والشراء بشكل منفصل. بالنسبة لعمليه الشراء لمره واحده ، سيقوم النموذج بتقليل التوقعات بعد مرور 10 أيام لحساب الزيادة المفاجئة في التكاليف

**ارغب في رؤية التنبؤات لبعد واحد (علي سبيل المثال. قراء**  
يدعم التنبؤ حاليا إسقاطات التكلفة الاجماليه وليس لأمتار الفردية. ولذلك ، عندما يكون ' تم التجميع حسب ' بعد ، سيكون الإسقاطات لإجمالي كل العناصر في البعد

**المستندات المستحسنة**

- [ما المقصود باداره التكاليف في Azure ؟](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [أفضل الممارسات لأداره التكاليف في Azure](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [تحليل التكاليف والانفاق](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [استكشاف التكاليف وتحليلها باستخدام تحليل التكلفة](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [أداره التكاليف في Azure: الأسعار](https://azure.microsoft.com/services/cost-management/#pricing)
- [مراجعه التكاليف في تحليل التكلفة](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [البرنامج التعليمي للفيديو: إنشاء موازنة في مدخل Azure](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [المتطلبات الاساسيه لعرض الموازنات وتخصيصها](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [إنشاء موازنات وأدارهها](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [تكوين التنفيذ التلقائي باستخدام مجموعات الإجراءات والموازنات في Azure](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [استخدام تنبيات التكلفة لمراقبه الاستخدام والانفاق](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [أفضل الممارسات لأداره التكاليف](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**مقاطع فيديو تعليمية**

- [إنشاء موازنة في مدخل Azure](https://go.microsoft.com/fwlink/?linkid=2146761)
- [أداره التكاليف باستخدام واجهه برمجه تطبيقات الموازنة ومجموعات الإجراءات](https://go.microsoft.com/fwlink/?linkid=2147038)