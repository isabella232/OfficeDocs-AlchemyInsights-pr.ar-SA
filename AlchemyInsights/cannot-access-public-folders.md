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
ms.openlocfilehash: f129da8731877aa00fd9b1dcf20905d353a4895303390ce7ff5642a8ff3ccbc2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53996617"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook الاتصال بالمجلدات العمومية

إذا لم يكن الوصول إلى المجلد العمومي يعمل مع بعض المستخدمين، فجرب ما يلي:

الاتصال EXO PowerShell وتكوين المعلمة DefaultPublicFolderMailbox على حساب المستخدم للمشكلة لمطابقة المعلمة في حساب مستخدم يعمل.

على سبيل المثال:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

انتظر ساعة واحدة على الأقل لكي يتم تغييره.

إذا بقيت المشكلة قائمة، فالرجاء اتباع [هذا الإجراء](https://aka.ms/pfcte) لا استكشاف مشاكل الوصول إلى المجلد العمومي وإصلاحها باستخدام Outlook.
 
**للتحكم في المستخدمين الذين يمكنهم الوصول إلى المجلدات العامة باستخدام Outlook:**

1.  استخدم Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true أو $false  
      
    $true: للسماح للمستخدمين بالوصول إلى المجلدات العامة في Outlook  
      
    $false: منع وصول المستخدم إلى المجلدات العامة في Outlook. هذه هي القيمة الافتراضية.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**ملاحظة** يمكن لهذا الإجراء التحكم في الاتصالات فقط Outlook سطح المكتب Windows العملاء. يمكن للمستخدم متابعة الوصول إلى المجلدات العامة باستخدام OWA أو Outlook for Mac.
 
لمزيد من المعلومات، راجع الإعلان عن دعم الاتصالات التي يتم التحكم فيها [بالمجلدات](https://aka.ms/controlpf)العامة في Outlook.