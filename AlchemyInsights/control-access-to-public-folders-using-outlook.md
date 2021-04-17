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
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="ea9a3-102">التحكم في الوصول إلى المجلدات العامة باستخدام Outlook</span><span class="sxs-lookup"><span data-stu-id="ea9a3-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="ea9a3-103">للتحكم في أي المستخدمين الذين يمكنهم الوصول إلى المجلدات العامة باستخدام Outlook:</span><span class="sxs-lookup"><span data-stu-id="ea9a3-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="ea9a3-104">استخدام `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="ea9a3-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="ea9a3-105">$true: للسماح للمستخدمين بالوصول إلى المجلدات العامة في Outlook</span><span class="sxs-lookup"><span data-stu-id="ea9a3-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="ea9a3-106">$false: منع وصول المستخدم إلى المجلدات العامة في Outlook.</span><span class="sxs-lookup"><span data-stu-id="ea9a3-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="ea9a3-107">هذه هي القيمة الافتراضية.</span><span class="sxs-lookup"><span data-stu-id="ea9a3-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="ea9a3-108">ملاحظة: هذا الإجراء لا يتحكم إلا في الاتصالات مع Outlook على سطح المكتب بالنسبة لعملاء Windows.</span><span class="sxs-lookup"><span data-stu-id="ea9a3-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="ea9a3-109">يمكن أن يستمر المستخدمون في الوصول إلى المجلدات الفرعية باستخدام OWA أو Outlook for Mac.</span><span class="sxs-lookup"><span data-stu-id="ea9a3-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="ea9a3-110">لمزيد من المعلومات، انظر [الاتصالات الخاضعة للتحكم بالمجلدات العامة في Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="ea9a3-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
