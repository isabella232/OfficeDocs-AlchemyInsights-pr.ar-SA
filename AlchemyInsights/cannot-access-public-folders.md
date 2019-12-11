---
title: لا يمكن الوصول إلى المجلدات العمومية
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
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959482"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>يتعذر علي Outlook الاتصال بالمجلدات العمومية

إذا كان الوصول إلى المجلد العمومي لا يعمل لعدد قليل من المستخدمين ، فجرب ما يلي:

الاتصال ب EXO PowerShell ، وتكوين ديفاولبوبليكفولدفولبوكس علي حساب المستخدم المشكلة لمطابقه واحد علي حساب مستخدم العمل.

المثال:

الحصول علي علبه البريد WorkingUser | ft ديفاولبوبليكفولدفولبوكس ، افيكتيفيبوبليكفولديرمايلبوكس

مجموعه-علبه البريد إشكاليه المستخدم-ديفاولبوبليكفولدفولبوكس \<من الأمر السابق>

انتظر ساعة واحده علي الأقل حتى يسري مفعول التغيير.