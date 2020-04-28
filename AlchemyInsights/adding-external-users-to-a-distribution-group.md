---
title: إضافة مستخدمين خارجيين إلى مجموعة توزيع
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 7dbc69bced9ca800d3f95081b77dda5e49662579
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/27/2020
ms.locfileid: "43910919"
---
# <a name="add-external-users-to-a-distribution-group"></a>إضافة مستخدمين خارجيين إلى مجموعة توزيع

إضافة جهة اتصال خارجية إلى مجموعة توزيع (DG) هي عملية من خطوتين:
  
1. إنشاء جهة اتصال بريد للمستخدم الخارجي:
    
    1. في مركز المشرف، انتقل إلى صفحة[جهات اتصال](https://admin.microsoft.com/adminportal/home#/Contact) **المستخدمين.** >  
    
    2. حدد **إضافة جهة اتصال**.
    
    3. اكتب المعلومات الخاصة بجهة الاتصال الخاصة بك وحدد **إضافة**.
    
2. إضافة جهة اتصال البريد إلى DG الخاص بك:
    
    1. في مركز المسؤول، انتقل إلى صفحة[مجموعات](https://admin.microsoft.com/adminportal/home#/groups) **المجموعات.** >  
    
    2. ابحث عن DG الذي تريد إضافة المستخدم الخارجي إليه، وحدده لفتح مربع حوار تحرير.
    
    3. في علامة التبويب **الأعضاء،** حدد **عرض الكل وإدارة الأعضاء**. 
    
    4. حدد **إضافة أعضاء**.
    
    5. حدد جهة اتصال البريد التي أنشأتها في الخطوة السابقة، ثم حدد **حفظ**.
    
إذا لم يتمكن المستخدمون الخارجيون بعد اتباع هذه الخطوات من إرسال رسائل البريد الإلكتروني إلى DG أو لم يتلقوا رسائل بريد إلكتروني منه، فقد يكون ذلك أن يتم وضع علامة على DG للسماح فقط برسائل البريد الإلكتروني من المستخدمين الداخليين. يمكنك التحقق من هذا التكوين وإصلاحه باتباع الاتجاهات [هنا](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **ملاحظة:** لا تنطبق هذه الإرشادات إذا كان نوع مجموعتك هو "مجموعة Microsoft 365" بدلاً من "مجموعة التوزيع". إذا كان هذا هو الحال، يمكنك إضافة المستخدم الخارجي مباشرة إلى المجموعة من Outlook. يمكن العثور على معلومات تفصيلية عن ضيوف مجموعات Microsoft 365 بالإضافة إلى إرشادات لإضافة ضيوف خارجيين في [هذه المقالة](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  