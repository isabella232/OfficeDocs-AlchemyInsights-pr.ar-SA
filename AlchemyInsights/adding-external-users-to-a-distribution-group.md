---
title: أضافه مستخدمين خارجيين إلى مجموعه توزيع
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663500"
---
# <a name="add-external-users-to-a-distribution-group"></a>أضافه مستخدمين خارجيين إلى مجموعه توزيع

تعد أضافه جهة اتصال خارجيه إلى مجموعه توزيع (توزيع) عمليه تتكون من خطوتين:
  
1. إنشاء جهة اتصال بريد للمستخدم الخارجي:
    
    1. في مركز الاداره ، انتقل إلى صفحه **Users**  >  [جات اتصال](https://admin.microsoft.com/adminportal/home#/Contact) المستخدمين. 
    
    2. حدد **أضافه جهة اتصال**.
    
    3. اكتب المعلومات الخاصة بجهة الاتصال وحدد **أضافه**.
    
2. أضف جهة الاتصال الخاصة بالبريد إلى توزيعك:
    
    1. في مركز الاداره ، انتقل إلى صفحه مجموعات **المجموعات**  >  [Groups](https://admin.microsoft.com/adminportal/home#/groups) . 
    
    2. ابحث عن توزيع الذي تريد أضافه المستخدم الخارجي اليه ، وحدده لفتح مربع الحوار تحرير.
    
    3. علي علامة التبويب **الأعضاء** ، حدد **عرض كل الأعضاء وأدارهم**. 
    
    4. حدد **أضافه أعضاء**.
    
    5. حدد جهة الاتصال التي انشاتها في الخطوة السابقة ، ثم حدد **حفظ**.
    
إذا لم يتمكن المستخدمون الخارجيون من تنفيذ الخطوات التالية من إرسال رسائل البريد الكتروني إلى توزيع أو عدم تلقي رسائل البريد الكتروني منه ، فقد يكون من الممكن وضع علامة علي التوزيع للسماح برسائل البريد الكتروني من المستخدمين الداخليين فقط. يمكنك التحقق من هذا التكوين وإصلاحه باتباع الإرشادات الواردة [هنا](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **ملاحظه:** لا تنطبق هذه الإرشادات إذا كان نوع المجموعة "Microsoft 365 group" بدلا من "مجموعه التوزيع". إذا كانت هذه هي الحالة ، يمكنك أضافه المستخدم الخارجي مباشره إلى المجموعة من Outlook. يمكن العثور علي معلومات مفصله حول ضيوف مجموعات Microsoft 365 بالاضافه إلى الإرشادات المتعلقة باضافه ضيوف خارجيين في [هذه المقالة](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  