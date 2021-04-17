---
title: يتعذر الوصول إلى المجلدات العامة
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819499"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>يتعذر على Outlook الاتصال بالمجلدات العامة

إذا لم يكن الوصول إلى المجلد العمومي يعمل مع بعض المستخدمين، فجرب ما يلي:

الاتصال ب EXO PowerShell وتكوين المعلمة DefaultPublicFolderMailbox على حساب المستخدم للمشكلة لمطابقة المعلمة على حساب مستخدم يعمل.

على سبيل المثال:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

انتظر ساعة واحدة على الأقل لكي يتم تغييره.

إذا بقيت المشكلة قائمة، فالرجاء اتباع [هذا الإجراء](https://aka.ms/pfcte) لا استكشاف مشاكل الوصول إلى المجلد العمومي وإصلاحها باستخدام Outlook.
 
**للتحكم في المستخدمين الذين يمكنهم الوصول إلى المجلدات العامة باستخدام Outlook:**

1.  استخدم Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true أو $false  
      
    $true: السماح للمستخدمين بالوصول إلى المجلدات العامة في Outlook  
      
    $false: منع وصول المستخدم إلى المجلدات العامة في Outlook. هذه هي القيمة الافتراضية.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**ملاحظة** يمكن لهذا الإجراء التحكم في الاتصالات فقط مع Outlook لسطح المكتب لعملاء Windows. يمكن للمستخدم متابعة الوصول إلى المجلدات العامة باستخدام OWA أو Outlook for Mac.
 
لمزيد من المعلومات، راجع الإعلان عن دعم الاتصالات التي يتم التحكم فيها [بالمجلدات العامة في Outlook](https://aka.ms/controlpf).