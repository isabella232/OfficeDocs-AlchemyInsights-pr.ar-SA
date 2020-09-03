---
title: تعذر الوصول إلى المجلدات العامة
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: d63a193585cb73c2ce8e160d413db4e837100d33
ms.sourcegitcommit: d3ace2376195d54229ee1e232daf8133ba4e58a9
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/03/2020
ms.locfileid: "47341390"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>يتعذر علي Outlook الاتصال بالمجلدات العامة

إذا لم يعمل الوصول إلى المجلد العام لبعض المستخدمين ، فجرب ما يلي:

اتصل ب أكسو PowerShell وقم بتكوين المعلمة ديفاولتبوبليكفولديرمايلبوكس علي حساب المستخدم الخاص بالمشكلة لمطابقه المعلمة علي حساب المستخدم الذي يعمل.

مثال

الحصول علي علبه البريد ووركينجوسير | ft ديفاولتبوبليكفولديرمايلبوكس ، افيكتيفيبوبليكفولديرمايلبوكس

تعيين-علبه البريد بروبليموسير-ديفاولتبوبليكفولديرمايلبوكس \<value from previous command>

انتظر حتى الآن ساعة واحده علي الأقل لكي يدخل التغيير حيز التنفيذ.

إذا استمرت المشكلة ، فالرجاء اتباع [هذا الاجراء](https://aka.ms/pfcte) لاستكشاف مشاكل الوصول إلى المجلد العام باستخدام Outlook وإصلاحها.
 
**للتحكم في المستخدمين الذين يمكنهم الوصول إلى المجلدات العامة باستخدام Outlook**:

1.  استخدام Set-casmailbox <mailboxname> -بوبليكفولديركلينتاكسيس $true أو $false  
      
    ال$true: السماح للمستخدمين بالوصول إلى المجلدات العامة في Outlook  
      
    $false: منع وصول المستخدم إلى المجلدات العمومية في Outlook. هذه هي القيمة الافتراضية.  
        
2.  Get-organizationconfig-بوبليكفولديرشووكلينتكونترول $true   
      
**ملاحظه** يمكن ان يتحكم هذا الاجراء بالاتصالات فقط باستخدام Outlook لسطح المكتب لعملاء Windows. يمكن للمستخدم الاستمرار في الوصول إلى المجلدات العامة باستخدام OWA أو Outlook for Mac.
 
للحصول علي مزيد من المعلومات ، راجع [دعم إعلانات الاتصال بالمجلدات العامة في Outlook](https://aka.ms/controlpf).