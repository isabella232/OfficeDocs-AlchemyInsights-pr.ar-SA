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
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816727"
---
# <a name="control-access-to-public-folders-using-outlook"></a>التحكم في الوصول إلى المجلدات العامة باستخدام Outlook

للتحكم في أي المستخدمين الذين يمكنهم الوصول إلى المجلدات العامة باستخدام Outlook:

1. استخدام `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: للسماح للمستخدمين بالوصول إلى المجلدات العامة في Outlook  
$false: منع وصول المستخدم إلى المجلدات العامة في Outlook. هذه هي القيمة الافتراضية.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

ملاحظة: هذا الإجراء لا يتحكم إلا في الاتصالات مع Outlook على سطح المكتب بالنسبة لعملاء Windows. يمكن أن يستمر المستخدمون في الوصول إلى المجلدات الفرعية باستخدام OWA أو Outlook for Mac.

لمزيد من المعلومات، انظر [الاتصالات الخاضعة للتحكم بالمجلدات العامة في Outlook](https://aka.ms/controlpf).
