---
title: يتعذر على المالك إنشاء مجلد فرعي باستخدام Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836122"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>يتعذر على المالك إنشاء مجلد فرعي باستخدام Outlook

**هناك مشكلة مستمرة في إنشاء مالكي المجلدات العمومية للمجلدات الفرعية باستخدام Outlook. سيتم إصلاح المشكلة قريبا.**

وفي هذه الأثناء، استخدم أحد الحلول التالية:

1. استخدم Outlook for MAC لإنشاء الملف الفرعي حيث تؤثر المشكلة على Outlook فقط على نوافذ سطح المكتب (كل الإصدارات)
2. هل يجب على المسؤول إنشاء المدوّن الفرعي باستخدام EXO Shell أو EAC
3. تغيير DefaultPublicFolderMailbox/EffectivePublicFolderMailbox على المستخدم إلى علبة بريد أخرى غير علبة بريد المحتوى للمجلد الذي تسبب المشكلة  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. انتظر لمدة ساعة، أعد تشغيل عميل outlook