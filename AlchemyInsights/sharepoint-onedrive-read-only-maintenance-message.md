---
title: للقراءة فقط لرسالة الصيانة عند محاولة استخدام SharePoint أو OneDrive
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
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670819"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>للقراءة فقط لرسالة الصيانة عند محاولة استخدام SharePoint أو OneDrive

قد يتلقى **المستخدمون للقراءة فقط لرسالة الصيانة** عند محاولة استخدام SharePoint أو OneDrive لأحدي السيناريوهات التالية. 

-   نشاط صيانة مخطط أو نشط.  ابحث عنها عن طريق الانتقال إلى [مركز الرسائل](https://portal.office.com/adminportal/home#/messagecenter).
-   حدث الخدمة ذات الاولويه العالية والفعالة التي قد تحدث. ابحث عن اي نصائح/حوادث عن طريق الانتقال إلى [حماية الخدمة](https://portal.office.com/adminportal/home#/servicehealth).
-   سيناريو الإصلاح التلقائي الثانوي الذي يمكن ان يحدث بسبب اي احداث غير متوقعه علي الخوادم التي قد تقل عن 30 دقيقه أو بالتالي. 
    
    لا توجد اي عمليات نشر لمركز الرسائل أو الخدمة لهذه الريكوفيريس الثانوية ولكن يجب ان تعود إلى الحالة العادية قريبا.

في حالات قليله جدا ، لقد قمنا بملاحظه ان أحدي السيناريوهات الثلاثة المدرجة أعلاه قد حدثت ، وتمت استعاده الخدمة ، ولكن لم يتم مسح ذاكره التخزين المؤقت لمستعرض المستخدمين.

يرجى محاولة مسح ذاكره التخزين المؤقت للمستعرض قبل التنقل إلى الموقع.

1. في مستعرض Microsoft Edge ، حدد **إعدادات**، ثم حدد **الخصوصية والأمان**.
2. ضمن **مسح الاستعراض**، حدد **اختيار ما تريد مسحه**.
3. حدد **ملفات تعريف الارتباط وبيانات موقع ويب محفوظه**، وحدد **مسح**.

>[!Note] 
> قد تختلف هذه الخطوات عند استخدام مستعرضات أخرى مثل Mozilla Firefox أو Google Chrome.

>[!Note] 
> هناك خيار آخر لفتح موقع SharePoint أو OneDrive في نافذه InPrivate جديده.