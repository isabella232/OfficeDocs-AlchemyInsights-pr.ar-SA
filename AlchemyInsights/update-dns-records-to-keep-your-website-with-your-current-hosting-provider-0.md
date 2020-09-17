---
title: تحديث سجلات DNS للاحتفاظ بموقعك علي ويب مع موفر الاستضافة الحالي
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 1d8654bc2dfb9063d0203992d624285eb646027d
ms.sourcegitcommit: 78939b01579b626b147d356045a37aec1170c948
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47815772"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>تحديث سجلات DNS للاحتفاظ بموقعك علي ويب مع موفر الاستضافة الحالي

1. في مركز أداره Microsoft 365 ، انتقل إلى صفحه **"إعدادات**  >  [المجالات](https://admin.microsoft.com/Adminportal#/Domains) " ، وفي قائمه المجالات ، حدد المجال الذي تستخدمه لموقعك علي ويب.

2. **حدد + سجل مخصص جديد** وادخل ما يلي:

  - بالنسبة إلى **نوع DNS** ، ادخل: **(عنوان)**

  - بالنسبة إلى **اسم المضيف أو الاسم المستعار**، اكتب ما يلي: **@**

  - بالنسبة إلى **عنوان ip**، اكتب عنوان ip الثابت لموقع ويب الخاص بك حيث تتم استضافته حاليا (علي سبيل المثال ،: 172.16.140.1).

    يجب ان يكون هذا عنوان ip  *ثابتا*  لموقع ويب ، وليس عنوان ip  *ديناميكي*  . راجع الموقع حيث تتم استضافه موقعك علي ويب للتاكد من انه يمكنك الحصول علي عنوان IP ثابت لموقعك العام علي ويب.

3. حدد **حفظ**.

بالاضافه إلى ذلك ، يمكنك إنشاء سجل CNAME لمساعده العملاء علي العثور علي موقعك علي ويب.
  
1. **حدد + سجل مخصص جديد** وادخل ما يلي:

  - بالنسبة إلى **نوع DNS** الإدخال: **CNAME (Alias)**

  - بالنسبة إلى **اسم المضيف أو الاسم المستعار**، اكتب ما يلي: **www**

  - بالنسبة **إلى العنوان**، اكتب اسم المجال المؤهل بالبالكامل (FQDN) لموقعك علي ويب (علي سبيل المثال ، contoso.com).

2. حدد **حفظ**.
