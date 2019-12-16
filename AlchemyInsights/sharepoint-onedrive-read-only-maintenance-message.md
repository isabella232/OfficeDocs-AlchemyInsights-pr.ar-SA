---
title: للقراءة فقط لرسالة الصيانة عند محاولة استخدام SharePoint أو اندريف
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051268"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>للقراءة فقط لرسالة الصيانة عند محاولة استخدام SharePoint أو اندريف

قد يتلقى المستخدمون **للقراءة فقط لرسالة الصيانة** عند محاولة استخدام SharePoint أو اندريف لأحد السيناريوهات التالية. 

-   نشاط صيانة مخطط أو نشط.  تحقق منها عن طريق الانتقال إلى [مركز الرسائل](https://portal.office.com/adminportal/home#/messagecenter).
-   حادثه خدمه نشطه ذات اولويه عاليه قد تحدث. التحقق من وجود اي نصائح/الحوادث عن طريق الانتقال إلى [خدمه الصحة](https://portal.office.com/adminportal/home#/servicehealth).
-   سيناريو استرداد الشفاء التلقائي البسيطة التي يمكن ان يحدث بسبب اي احداث غير متوقعه علي الملقمات التي قد تستمر لمده اقل من 30 دقيقه أو نحو ذلك. 
    
    لا توجد مراكز الرسائل أو الخدمات الصحية المشاركات لهذه المبالغ المستردة البسيطة ولكن يجب ان تكون العودة إلى طبيعتها قريبا جدا.

في مناسبات قليله جدا لاحظنا ان واحدا من السيناريوهات الثلاثة المذكورة أعلاه كان السبب ، وتم استعاده الخدمة ، ولكن لم يتم مسح ذاكره التخزين المؤقت للمتصفح المستخدمين.

الرجاء محاولة مسح ذاكره التخزين المؤقت للمتصفح قبل الانتقال إلى الموقع.

1. في مستعرض Microsoft Edge ، حدد **الإعدادات**، ثم حدد **الخصوصية والأمان**.
2. ضمن **استعراض واضح**، حدد **اختيار ما تريد إلغاء**تحديده.
3. حدد **ملفات تعريف الارتباط وبيانات موقع الويب المحفوظة**، ثم اختر **مسح**.

>[!Note] 
> قد تختلف هذه الخطوات عند استخدام متصفحات أخرى مثل موزيلا فايرفوكس أو جوجل كروم.

>[!Note] 
> سيكون خيار آخر لفتح موقع SharePoint أو اندريف في اطار InPrivate جديد.