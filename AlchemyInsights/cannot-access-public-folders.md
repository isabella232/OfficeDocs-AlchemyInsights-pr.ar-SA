---
title: تعذر الوصول إلى المجلدات العامة
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812534"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="8fa5d-102">يتعذر علي Outlook الاتصال بالمجلدات العامة</span><span class="sxs-lookup"><span data-stu-id="8fa5d-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="8fa5d-103">إذا لم يعمل الوصول إلى المجلد العام لبعض المستخدمين ، فجرب ما يلي:</span><span class="sxs-lookup"><span data-stu-id="8fa5d-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="8fa5d-104">اتصل ب أكسو PowerShell وقم بتكوين المعلمة ديفاولتبوبليكفولديرميلبوكس علي حساب المستخدم الخاص بالمشكلة لمطابقه المعلمة علي حساب المستخدم الذي يعمل.</span><span class="sxs-lookup"><span data-stu-id="8fa5d-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="8fa5d-105">مثال</span><span class="sxs-lookup"><span data-stu-id="8fa5d-105">Example:</span></span>

<span data-ttu-id="8fa5d-106">الحصول علي علبه البريد ووركينجوسير | ft ديفاولتبوبليكفولديرميلبوكس ، افيكتيفيبوبليكفولديرمايلبوكس</span><span class="sxs-lookup"><span data-stu-id="8fa5d-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="8fa5d-107">تعيين-علبه البريد بروبليموسير-ديفاولتبوبليكفولديرميلبوكس \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="8fa5d-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="8fa5d-108">انتظر حتى الآن ساعة واحده علي الأقل لكي يدخل التغيير حيز التنفيذ.</span><span class="sxs-lookup"><span data-stu-id="8fa5d-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="8fa5d-109">إذا استمرت المشكلة ، فالرجاء اتباع [هذا الاجراء](https://aka.ms/pfcte) لاستكشاف مشاكل الوصول إلى المجلد العام باستخدام Outlook وإصلاحها.</span><span class="sxs-lookup"><span data-stu-id="8fa5d-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="8fa5d-110">**للتحكم في المستخدمين الذين يمكنهم الوصول إلى المجلدات العامة باستخدام Outlook**:</span><span class="sxs-lookup"><span data-stu-id="8fa5d-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="8fa5d-111">استخدام Set-casmailbox <mailboxname> -بوبليكفولديركلينتاكسيس $true أو $false</span><span class="sxs-lookup"><span data-stu-id="8fa5d-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="8fa5d-112">ال$true: السماح للمستخدمين بالوصول إلى المجلدات العامة في Outlook</span><span class="sxs-lookup"><span data-stu-id="8fa5d-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="8fa5d-113">$false: منع وصول المستخدم إلى المجلدات العمومية في Outlook.</span><span class="sxs-lookup"><span data-stu-id="8fa5d-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="8fa5d-114">هذه هي القيمة الافتراضية.</span><span class="sxs-lookup"><span data-stu-id="8fa5d-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="8fa5d-115">Get-organizationconfig-بوبليكفولديرشووكلينتكونترول $true</span><span class="sxs-lookup"><span data-stu-id="8fa5d-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="8fa5d-116">**ملاحظه** يمكن ان يتحكم هذا الاجراء بالاتصالات فقط باستخدام Outlook لسطح المكتب لعملاء Windows.</span><span class="sxs-lookup"><span data-stu-id="8fa5d-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="8fa5d-117">يمكن للمستخدم الاستمرار في الوصول إلى المجلدات العامة باستخدام OWA أو Outlook for Mac.</span><span class="sxs-lookup"><span data-stu-id="8fa5d-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="8fa5d-118">للحصول علي مزيد من المعلومات ، راجع [دعم إعلانات الاتصال بالمجلدات العامة في Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="8fa5d-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>