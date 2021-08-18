---
title: Read-Only رسالة الصيانة عند محاولة استخدام SharePoint أو OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 376b653b18857103586e25edd0ad6801a7bbe0a1
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329435"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Read-Only رسالة الصيانة عند محاولة استخدام SharePoint أو OneDrive

قد يتلقى المستخدمون رسالة للقراءة **فقط** للصيانة عند محاولة استخدام SharePoint أو OneDrive لأحد السيناريوهات التالية. 

-   نشاط صيانة مخطط له أو نشط.  تحقق من ذلك من خلال الانتقال إلى [مركز الرسائل](https://portal.office.com/adminportal/home#/messagecenter).
-   حدث خدمة نشط عالي الأولوية قد يحدث. تحقق من وجود أي استشارات/أحداث من خلال الانتقال إلى ["صحة الخدمة".](https://portal.office.com/adminportal/home#/servicehealth)
-   سيناريو استرداد تلقائي بسيط قد يحدث بسبب أي أحداث غير متوقعة على الخوادم قد تستمر لأقل من 30 دقيقة أو نحو ذلك. 
    
    لا توجد منشورات مركز الرسائل أو "صحة الخدمة" لهذه عمليات استرداد بسيطة ولكن من المفترض أن تعود إلى الوضع العادي في وقت قريب جدا.

في حالات قليلة جدا، لاحظنا أن أحد السيناريوهات الثلاثة المذكورة أعلاه كان السبب، وقد تم استعادة الخدمة، ولكن لم يتم مسح ذاكرة التخزين المؤقت لمستعرض المستخدمين.

الرجاء محاولة مسح ذاكرة التخزين المؤقت للمستعرض قبل الانتقال إلى الموقع.

1. في المستعرض Microsoft Edge، **حدد** الإعدادات ، ثم حدد **الخصوصية والأمان**.
2. ضمن **مسح الاستعراض،** **حدد اختيار ما تريد مسحه.**
3. حدد **ملفات تعريف الارتباط وبيانات موقع الويب المحفوظة**، وحدد **مسح**.

**ملاحظة:** قد تختلف هذه الخطوات عند استخدام مستعرضات أخرى مثل Mozilla Firefox أو Google Chrome.

**ملاحظة**: هناك خيار آخر وهو فتح SharePoint أو OneDrive في نافذة InPrivate جديدة.