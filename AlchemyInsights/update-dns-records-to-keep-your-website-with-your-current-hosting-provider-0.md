---
title: تحديث سجلات DNS للحفاظ على موقع الويب الخاص بك باستخدام موفر الاستضافة الحالية
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: e0dadba1e3ffd1cf0d49c0a76ec2efbbc6ae92db
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29906107"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>تحديث سجلات DNS للحفاظ على موقع الويب الخاص بك باستخدام موفر الاستضافة الحالية

1. على الصفحة " [مجالات](https://portal.office.com/adminportal/home#/Domains) "، في قائمة المجالات، حدد المجال الذي تستخدمه لموقع الويب الخاص بك، وثم حدد **إعدادات DNS** في جزء "إدارة". 
    
2. حدد **+ سجل مخصص جديد** وأدخل ما يلي: 
    
  - أدخل نوع **DNS** : **(عنوان)**
    
  - **اسم المضيف أو اسم مستعار**، اكتب ما يلي:**@**
    
  - **عنوان IP**، اكتب عنوان IP لموقع الويب الخاص بك حيث يتم حاليا استضافته (على سبيل المثال، 172.16.140.1). 
    
    يجب أن يكون عنوان IP *ثابت* لموقع ويب، وليس عنوان IP *حيوي* . تحقق من الموقع حيث استضافة موقع الويب الخاص بك للتأكد من أنه يمكنك الحصول على عنوان IP ثابت لموقع الويب العمومي الخاص بك. 
    
3. حدد **حفظ**. 
    
وبالإضافة إلى ذلك، يمكنك إنشاء سجل CNAME لمساعدة العملاء على العثور على موقع الويب الخاص بك.
  
1. حدد **+ سجل مخصص جديد** وأدخل ما يلي: 
    
  - أدخل نوع **DNS** : **CNAME (اسم مستعار)**
    
  - **اسم المضيف أو اسم مستعار**، اكتب ما يلي: **www**
    
  - **يشير إلى عنوان**، اكتب اسم المجال المؤهل بالكامل (FQDN) لموقع الويب الخاص بك (على سبيل المثال، "contoso.com" أيضا). 
    
2. حدد **حفظ**. 
    

