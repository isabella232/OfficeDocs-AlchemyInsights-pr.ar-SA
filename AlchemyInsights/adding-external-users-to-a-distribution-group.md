---
title: إضافة مستخدمين خارجيين إلى مجموعة توزيع
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: d8c06c81ecc66df0fbaa4cac9908178cdc1d9c6bdc38d19010c7b55e9bca8776
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934820"
---
# <a name="add-external-users-to-a-distribution-group"></a>إضافة مستخدمين خارجيين إلى مجموعة توزيع

تتم عملية إضافة جهة اتصال خارجية إلى مجموعة توزيع (DG) على خطوتين:
  
1. إنشاء جهة اتصال بريد للمستخدم الخارجي:
    
    1. في مركز الإدارة، انتقل إلى صفحة **جهات اتصال**  >  [](https://admin.microsoft.com/adminportal/home#/Contact) المستخدمين. 
    
    2. حدد **إضافة جهة اتصال**.
    
    3. اكتب معلومات جهة الاتصال وحدد **إضافة**.
    
2. إضافة جهة اتصال البريد إلى DG:
    
    1. في مركز الإدارة، انتقل إلى صفحة  >  [مجموعات](https://admin.microsoft.com/adminportal/home#/groups) المجموعات. 
    
    2. ابحث عن مجموعة DG التي تريد إضافة المستخدم الخارجي لها، ثم حددها لفتح مربع الحوار تحرير.
    
    3. على علامة **التبويب** الأعضاء، حدد **عرض الكل وإدارة الأعضاء**. 
    
    4. حدد **إضافة أعضاء**.
    
    5. حدد جهة اتصال البريد التي أنشأتها في الخطوة السابقة، ثم حدد **حفظ**.
    
إذا لم تتمكن المستخدمون الخارجيون من إرسال رسائل بريد إلكتروني إلى DG أو لم يتلقوا رسائل بريد إلكتروني منها بعد اتباع هذه الخطوات، فقد يتم وضع علامة على DG للسماح فقط بإرسال رسائل البريد الإلكتروني من مستخدمين داخليين. يمكنك التحقق من هذا التكوين وإصلاحه باتباع التوجيهات [هنا](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **ملاحظة:** لا تنطبق هذه الإرشادات إذا كان نوع المجموعة "مجموعة Microsoft 365" بدلا من "مجموعة التوزيع". إذا كان الأمر كذلك، يمكنك إضافة المستخدم الخارجي مباشرة إلى المجموعة من Outlook. يمكن العثور على Microsoft 365 حول ضيوف المجموعات بالإضافة إلى إرشادات لإضافة ضيوف خارجيين في [هذه المقالة](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  