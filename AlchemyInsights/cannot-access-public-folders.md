---
title: تعذر الوصول إلى المجلدات العامة
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
ms.openlocfilehash: d63a193585cb73c2ce8e160d413db4e837100d33
ms.sourcegitcommit: d3ace2376195d54229ee1e232daf8133ba4e58a9
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/03/2020
ms.locfileid: "47341390"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="b8097-102">يتعذر علي Outlook الاتصال بالمجلدات العامة</span><span class="sxs-lookup"><span data-stu-id="b8097-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="b8097-103">إذا لم يعمل الوصول إلى المجلد العام لبعض المستخدمين ، فجرب ما يلي:</span><span class="sxs-lookup"><span data-stu-id="b8097-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="b8097-104">اتصل ب أكسو PowerShell وقم بتكوين المعلمة ديفاولتبوبليكفولديرمايلبوكس علي حساب المستخدم الخاص بالمشكلة لمطابقه المعلمة علي حساب المستخدم الذي يعمل.</span><span class="sxs-lookup"><span data-stu-id="b8097-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="b8097-105">مثال</span><span class="sxs-lookup"><span data-stu-id="b8097-105">Example:</span></span>

<span data-ttu-id="b8097-106">الحصول علي علبه البريد ووركينجوسير | ft ديفاولتبوبليكفولديرمايلبوكس ، افيكتيفيبوبليكفولديرمايلبوكس</span><span class="sxs-lookup"><span data-stu-id="b8097-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="b8097-107">تعيين-علبه البريد بروبليموسير-ديفاولتبوبليكفولديرمايلبوكس \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="b8097-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="b8097-108">انتظر حتى الآن ساعة واحده علي الأقل لكي يدخل التغيير حيز التنفيذ.</span><span class="sxs-lookup"><span data-stu-id="b8097-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="b8097-109">إذا استمرت المشكلة ، فالرجاء اتباع [هذا الاجراء](https://aka.ms/pfcte) لاستكشاف مشاكل الوصول إلى المجلد العام باستخدام Outlook وإصلاحها.</span><span class="sxs-lookup"><span data-stu-id="b8097-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="b8097-110">**للتحكم في المستخدمين الذين يمكنهم الوصول إلى المجلدات العامة باستخدام Outlook**:</span><span class="sxs-lookup"><span data-stu-id="b8097-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="b8097-111">استخدام Set-casmailbox <mailboxname> -بوبليكفولديركلينتاكسيس $true أو $false</span><span class="sxs-lookup"><span data-stu-id="b8097-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="b8097-112">ال$true: السماح للمستخدمين بالوصول إلى المجلدات العامة في Outlook</span><span class="sxs-lookup"><span data-stu-id="b8097-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="b8097-113">$false: منع وصول المستخدم إلى المجلدات العمومية في Outlook.</span><span class="sxs-lookup"><span data-stu-id="b8097-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="b8097-114">هذه هي القيمة الافتراضية.</span><span class="sxs-lookup"><span data-stu-id="b8097-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="b8097-115">Get-organizationconfig-بوبليكفولديرشووكلينتكونترول $true</span><span class="sxs-lookup"><span data-stu-id="b8097-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="b8097-116">**ملاحظه** يمكن ان يتحكم هذا الاجراء بالاتصالات فقط باستخدام Outlook لسطح المكتب لعملاء Windows.</span><span class="sxs-lookup"><span data-stu-id="b8097-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="b8097-117">يمكن للمستخدم الاستمرار في الوصول إلى المجلدات العامة باستخدام OWA أو Outlook for Mac.</span><span class="sxs-lookup"><span data-stu-id="b8097-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="b8097-118">للحصول علي مزيد من المعلومات ، راجع [دعم إعلانات الاتصال بالمجلدات العامة في Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="b8097-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>