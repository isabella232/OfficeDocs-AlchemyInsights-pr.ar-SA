---
title: إضافة مستخدمين خارجيين إلى مجموعة توزيع
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: e84a5b04d6fc805deaa47cb10c91081f37411e5b
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737860"
---
# <a name="add-external-users-to-a-distribution-group"></a>إضافة مستخدمين خارجيين إلى مجموعة توزيع

إضافة جهة اتصال خارجية إلى مجموعة توزيع (DG) عملية من خطوتين:
  
1. إنشاء جهة اتصال بريد للمستخدم الخارجي:
    
    1. في مركز المسؤول، انتقل إلى صفحة["جهات اتصال](https://admin.microsoft.com/adminportal/home#/Contact) **المستخدمين".** >  
    
    2. حدد **إضافة جهة اتصال**.
    
    3. اكتب المعلومات لجهة الاتصال الخاصة بك وحدد **إضافة**.
    
2. إضافة جهة اتصال البريد إلى المديرية العامة:
    
    1. في مركز المسؤول، انتقل إلى صفحة[مجموعات](https://admin.microsoft.com/adminportal/home#/groups) **المجموعات.** >  
    
    2. ابحث عن المدير ية التي تريد إضافة المستخدم الخارجي إليها، وحددها لفتح مربع حوار التحرير.
    
    3. في علامة التبويب **الأعضاء،** حدد **عرض الكل وإدارة الأعضاء**. 
    
    4. حدد **إضافة أعضاء**.
    
    5. حدد جهة اتصال البريد التي قمت بإنشائها في الخطوة السابقة، ثم حدد **حفظ**.
    
إذا لم يتمكن المستخدمون الخارجيون بعد اتباع هذه الخطوات من إرسال رسائل بريد إلكتروني إلى المديرية العامة أو عدم تلقي رسائل البريد الإلكتروني منها، فقد يكون من الممكن وضع علامة على المديرية العامة للسماح برسائل البريد الإلكتروني من المستخدمين الداخليين فقط. يمكنك التحقق من هذا التكوين وإصلاحه باتباع الإرشادات [هنا](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **ملاحظة:** لا يتم تطبيق هذه الإرشادات إذا كان نوع المجموعة الخاصة بك هو "مجموعة Office 365" بدلاً من "مجموعة التوزيع". إذا كانت هذه هي الحالة، يمكنك إضافة المستخدم الخارجي مباشرة إلى المجموعة من Outlook. يمكن العثور على معلومات مفصلة عن ضيوف مجموعات Office 365 وكذلك إرشادات لإضافة ضيوف خارجيين في [هذه المقالة](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  