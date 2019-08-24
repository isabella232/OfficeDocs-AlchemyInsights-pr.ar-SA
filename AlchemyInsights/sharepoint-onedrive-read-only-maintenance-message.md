---
title: القراءة فقط لصيانة رسالة عند محاولة استخدام SharePoint أو أندريف
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620710"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>القراءة فقط لصيانة رسالة عند محاولة استخدام SharePoint أو أندريف

ظهور رسالة **القراءة فقط للحفاظ على** المستخدمين عند محاولة استخدام SharePoint أو أندريف لأحد السيناريوهات التالية. 

-   بنشاط صيانة المخططة أو غير نشط.  البحث عنها عن طريق الانتقال إلى [مركز الرسائل](https://portal.office.com/adminportal/home#/messagecenter).
-   حادث خدمة النشطة ذات أولوية عالية، التي قد تحدث. التحقق من وجود أية نصائح/الحوادث المتعلقة بالتنقل إلى [الخدمات الصحية](https://portal.office.com/adminportal/home#/servicehealth).
-   ثانوية الإصلاح تلقائي استرداد سيناريو الذي قد يحدث نتيجة لأي أحداث غير متوقعة على الخوادم التي قد تستمر لمدة تقل عن 30 دقيقة أو نحو ذلك. 
    
    هناك لا مركز أو وظائف "الحماية خدمة" لهذه المبالغ المستردة الثانوية لكن يجب أن تكون العودة إلى طبيعتها قريبا جداً.

وفي حالات قليلة جداً أننا لاحظنا أن أحد السيناريوهات الثلاثة المذكورة أعلاه هي سبب، وتمت استعادة الخدمة، ولكن لم يتم مسح التخزين المؤقت للمستعرض المستخدمين.

الرجاء محاولة مسح التخزين المؤقت للمستعرض قبل الانتقال إلى الموقع.

1. في مستعرض حافة Microsoft، حدد **إعدادات**، وحدد **الخصوصية والأمان**.
2. ضمن **الاستعراض واضحة**، حدد **اختر ما تريد مسح**.
3. حدد **ملفات تعريف الارتباط وبيانات موقع ويب المحفوظة**، وحدد **مسح**.

>[!Note] 
> قد تختلف الخطوات التالية عند استخدام المستعرضات الأخرى مثل موزيلا فايرفوكس أو جوجل كروم.

>[!Note] 
> خيار آخر يتمثل في فتح موقع SharePoint الخاص بك أو أندريف في نافذة جديدة InPrivate.