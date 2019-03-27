---
title: استكشاف أخطاء مزامنة كلمات المرور
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 1320c0fe839337188162824439be6f15f86b6c90
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/22/2019
ms.locfileid: "30767163"
---
# <a name="troubleshoot-password-synchronization"></a>استكشاف أخطاء مزامنة كلمات المرور

لاستكشاف مشكلات فيها لم كلمات مرور متزامنة مع إصدار الاتصال الإعلان Azure 1.1.614.0 أو أحدث:
  
1. فتح جلسة عمل Windows PowerShell جديدة على ملقم الاتصال الإعلان Azure مع الخيار **تشغيل كمسؤول** . 
    
2. تشغيل **مجموعة ExecutionPolicy RemoteSigned** أو **مجموعة ExecutionPolicy غير مقيد**. 
    
3. بدء تشغيل معالج اتصال AD Azure.
    
4. انتقل إلى * * "مهام إضافية" * * الصفحة، حدد * * استكشاف * *، ثم انقر فوق **التالي**. 
    
5. في الصفحة استكشاف الأخطاء وإصلاحها، انقر فوق قائمة **التشغيل لبدء استكشاف الأخطاء وإصلاحها** في PowerShell. 
    
6. في القائمة الرئيسية، حدد **استكشاف أخطاء مزامنة كلمات المرور**. 
    
7. في القائمة الفرعية، حدد **"كلمة المرور المزامنة" لا تعمل على الإطلاق**. 
    
 **فهم نتائج مهمة استكشاف الأخطاء وإصلاحها**
  
مهمة استكشاف الأخطاء وإصلاحها يقوم بتنفيذ الاختبارات التالية:
  
- التحقق من تمكين ميزة مزامنة كلمة المرور للمستأجر Azure الإعلان الخاص بك.
    
- التحقق من أن الملقم الاتصال الإعلان Azure ليس في إعداد وضع.
    
- لكل القائمة الداخلية Active Directory الموصل (الذي يقابل إلى مجموعة تفرعات "Active Directory" موجودة):
    
- 
  - التحقق من تمكين ميزة مزامنة كلمة المرور.
    
  - البحث عن أحداث نبضات المزامنة كلمة المرور في سجلات Windows Application Event.
    
  - لكل مجال Active Directory ضمن موصل "خدمة active Directory" الداخلي:
    
  - التحقق من صحة المجال قابل من الملقم الاتصال الإعلان Azure.
    
  - التحقق من وجود حسابات "خدمات مجال خدمة active Directory" (AD DS) المستخدمة بواسطة موصل "خدمة active Directory" على أماكن العمل اسم المستخدم الصحيح وكلمة المرور والأذونات المطلوبة لمزامنة كلمات المرور.
    
لمزيد من استكشاف الأخطاء وإصلاحها مزامنة كلمة المرور، راجع [استكشاف الأخطاء وإصلاحها مزامنة كلمات المرور مع تزامن الاتصال الإعلان Azure](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  

