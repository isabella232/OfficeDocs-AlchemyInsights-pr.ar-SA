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
ms.openlocfilehash: 60190727e75c120ad3915da8b563b7f6b1a3238b46bb6e14cbf956365e1a84e0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54063111"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>يتعذر على المالك إنشاء مجلد فرعي باستخدام Outlook

**هناك مشكلة مستمرة في إنشاء مالكي المجلدات العامة للمجلدات الفرعية باستخدام Outlook. سيتم إصلاح المشكلة قريبا.**

وفي هذه الأثناء، استخدم أحد الحلول التالية:

1. استخدم Outlook ل MAC لإنشاء الملف الفرعي حيث تؤثر المشكلة فقط على Outlook Windows لسطح المكتب (كل الإصدارات)
2. هل يجب على المسؤول إنشاء المدوّن الفرعي باستخدام EXO Shell أو EAC
3. تغيير DefaultPublicFolderMailbox/EffectivePublicFolderMailbox على المستخدم إلى علبة بريد أخرى غير علبة بريد المحتوى للمجلد الذي تسبب المشكلة  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. انتظر لمدة ساعة، أعد تشغيل عميل outlook