---
title: لا يمكن الوصول إلى المجلدات العامة
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
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891736"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>لا يمكن لـ Outlook الاتصال بالمجلدات العامة

إذا كان الوصول إلى المجلد العمومي لا يعمل لبعض المستخدمين، فجرّب ما يلي:

الاتصال EXO PowerShell وتكوين المعلمة DefaultPublicFolderMailbox على حساب المستخدم المشكلة لمطابقة المعلمة على حساب مستخدم عامل.

المثال:

الحصول على علبة البريد المستخدم | ft DefaultPublicFolderMailbox، EffectivePublicFolderMailbox

مجموعة علبة البريد مشكلةUser \<-DefaultPublicFolderMailbox قيمة من الأمر السابق>

انتظر ساعة واحدة على الأقل حتى يسري التغيير.

إذا ظلت المشكلة قائمة، الرجاء اتباع [هذا الإجراء](https://aka.ms/pfcte) لاستكشاف مشاكل الوصول إلى المجلد العمومي باستخدام Outlook.