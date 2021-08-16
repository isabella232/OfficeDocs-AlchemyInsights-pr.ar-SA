---
title: التحكم في الوصول إلى المجلدات العامة باستخدام Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 1386b97f804e63455094abf64b9d9e2541d57dafa36535813b0d7689e0ce2966
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54032545"
---
# <a name="control-access-to-public-folders-using-outlook"></a>التحكم في الوصول إلى المجلدات العامة باستخدام Outlook

للتحكم في أي المستخدمين الذين يمكنهم الوصول إلى المجلدات العامة باستخدام Outlook:

1. استخدام `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: للسماح للمستخدمين بالوصول إلى المجلدات العامة في Outlook  
$false: منع وصول المستخدم إلى المجلدات العامة في Outlook. هذه هي القيمة الافتراضية.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

ملاحظة: هذا الإجراء لا يتحكم إلا في الاتصالات مع Outlook على سطح المكتب بالنسبة لعملاء Windows. يمكن أن يستمر المستخدمون في الوصول إلى المجلدات الفرعية باستخدام OWA أو Outlook for Mac.

لمزيد من المعلومات، انظر [الاتصالات الخاضعة للتحكم بالمجلدات العامة في Outlook](https://aka.ms/controlpf).
