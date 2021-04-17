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
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="5d273-102">يتعذر على Outlook الاتصال بالمجلدات العامة</span><span class="sxs-lookup"><span data-stu-id="5d273-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="5d273-103">إذا لم يكن الوصول إلى المجلد العمومي يعمل مع بعض المستخدمين، فجرب ما يلي:</span><span class="sxs-lookup"><span data-stu-id="5d273-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="5d273-104">الاتصال ب EXO PowerShell وتكوين المعلمة DefaultPublicFolderMailbox على حساب المستخدم للمشكلة لمطابقة المعلمة على حساب مستخدم يعمل.</span><span class="sxs-lookup"><span data-stu-id="5d273-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="5d273-105">على سبيل المثال:</span><span class="sxs-lookup"><span data-stu-id="5d273-105">Example:</span></span>

<span data-ttu-id="5d273-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="5d273-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="5d273-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="5d273-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="5d273-108">انتظر ساعة واحدة على الأقل لكي يتم تغييره.</span><span class="sxs-lookup"><span data-stu-id="5d273-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="5d273-109">إذا بقيت المشكلة قائمة، فالرجاء اتباع [هذا الإجراء](https://aka.ms/pfcte) لا استكشاف مشاكل الوصول إلى المجلد العمومي وإصلاحها باستخدام Outlook.</span><span class="sxs-lookup"><span data-stu-id="5d273-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="5d273-110">**للتحكم في المستخدمين الذين يمكنهم الوصول إلى المجلدات العامة باستخدام Outlook:**</span><span class="sxs-lookup"><span data-stu-id="5d273-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="5d273-111">استخدم Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true أو $false</span><span class="sxs-lookup"><span data-stu-id="5d273-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="5d273-112">$true: السماح للمستخدمين بالوصول إلى المجلدات العامة في Outlook</span><span class="sxs-lookup"><span data-stu-id="5d273-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="5d273-113">$false: منع وصول المستخدم إلى المجلدات العامة في Outlook.</span><span class="sxs-lookup"><span data-stu-id="5d273-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="5d273-114">هذه هي القيمة الافتراضية.</span><span class="sxs-lookup"><span data-stu-id="5d273-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="5d273-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="5d273-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="5d273-116">**ملاحظة** يمكن لهذا الإجراء التحكم في الاتصالات فقط مع Outlook لسطح المكتب لعملاء Windows.</span><span class="sxs-lookup"><span data-stu-id="5d273-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="5d273-117">يمكن للمستخدم متابعة الوصول إلى المجلدات العامة باستخدام OWA أو Outlook for Mac.</span><span class="sxs-lookup"><span data-stu-id="5d273-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="5d273-118">لمزيد من المعلومات، راجع الإعلان عن دعم الاتصالات التي يتم التحكم فيها [بالمجلدات العامة في Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="5d273-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>