---
title: تم رفض الوصول عند تعيين محرك أقراص إلى SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: c41bfd9d25c8aa946a4ec5156be6d2424f4e2133
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/18/2019
ms.locfileid: "36737464"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a>إصلاح مشاكل مع مكتبات SharePoint المعينة إلى محركات أقراص الشبكة

عند الاستعراض إلى محرك أقراص شبكه معين قد تري أحدي الرسائل التالية:
  
- **\\المسار غير قابل للوصول. قد لا يكون لديك الاذن باستخدام مورد شبكه الاتصال هذا. اتصل بمسؤول هذا الملقم لمعرفه ما إذا كان لديك أذونات الوصول.**

- **تم رفض الوصول. قبل فتح الملفات في هذا الموقع ، يجب أولا أضافه موقع ويب إلى قائمه المواقع الموثوق بها ، والاستعراض إلى موقع الويب ، وتحديد الخيار لتسجيل الدخول تلقائيا.**

[الحصول علي تعليمات استكشاف أخطاء محركات أقراص الشبكة المعينة](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).
  
تعيين مكتبه كمحرك أقراص شبكه مؤقت ومعتمد فقط في Internet Explorer. بدلا من ذلك ، [مزامنة ملفات SharePoint مع عميل المزامنة اندريف الجديد](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) الذي يتضمن [الملفات عند الطلب](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx). الوصول إلى كافة الملفات الخاصة بك في OneDrive دون استخدام مساحة التخزين المحلية.
  