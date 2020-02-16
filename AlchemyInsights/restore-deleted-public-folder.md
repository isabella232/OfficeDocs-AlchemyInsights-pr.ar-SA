---
title: استعادة مجلد عام محذوف
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
- "3488"
ms.openlocfilehash: 7b04612daca61650d162c1dde240e25c1b185b04
ms.sourcegitcommit: 8ba12eff67e405f5922ea4cc35155e3036447859
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2020
ms.locfileid: "42063580"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="987ba-102">استعادة مجلد عام محذوف</span><span class="sxs-lookup"><span data-stu-id="987ba-102">Restore a deleted public folder</span></span>

<span data-ttu-id="987ba-103">**لاستعادة العناصر المحذوفة من مجلد عام:**</span><span class="sxs-lookup"><span data-stu-id="987ba-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="987ba-104">راجع [لا يمكنك استرداد العناصر المحذوفة من مجلد عام غير بريد في Outlook 2016](https://aka.ms/pfrec).</span><span class="sxs-lookup"><span data-stu-id="987ba-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="987ba-105">**لاستعادة مجلد عام محذوف (من أي نوع):**</span><span class="sxs-lookup"><span data-stu-id="987ba-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="987ba-106">الرجاء استخدام الأمر EXO PowerShell التالي:</span><span class="sxs-lookup"><span data-stu-id="987ba-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="987ba-107">بناء الجمله:</span><span class="sxs-lookup"><span data-stu-id="987ba-107">Syntax:</span></span>

    ><span data-ttu-id="987ba-108">$pf = الحصول على PublicFolder \NON_IPM_SUBTREE \DUMPSTER_ROOT -recurse | ؟ {$_. اسم -eq\<"name_of_deleted_public_Folder"}؛ Set-PublicFolder $pf.identity-مسار \<حيث سيتم استعادة المجلد></span><span class="sxs-lookup"><span data-stu-id="987ba-108">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored></span></span>

    <span data-ttu-id="987ba-109">مثال: سيقوم الأمر التالي باستعادة المجلد الفرعي1 ووضعه تحت \Parent1:</span><span class="sxs-lookup"><span data-stu-id="987ba-109">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    ><span data-ttu-id="987ba-110">$pf = الحصول على PublicFolder \NON_IPM_SUBTREE \DUMPSTER_ROOT -recurse | ؟ {$_. اسم -eq "subfolder1"}; تعيين-PublicFolder $pf.الهوية -مسار \Parent1</span><span class="sxs-lookup"><span data-stu-id="987ba-110">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1</span></span>

<span data-ttu-id="987ba-111">راجع [استعادة مجلد عام محذوف](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) لمزيد من التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="987ba-111">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
