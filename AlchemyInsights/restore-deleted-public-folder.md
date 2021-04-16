---
title: استعادة مجلد عمومي محذوف
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
- "3488"
ms.openlocfilehash: d5480389c3bf50cee9fe30f7ec8d8ff28ef694ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809426"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="03871-102">استعادة مجلد عمومي محذوف</span><span class="sxs-lookup"><span data-stu-id="03871-102">Restore a deleted public folder</span></span>

<span data-ttu-id="03871-103">**لاستعادة العناصر المحذوفة من مجلد عمومي:**</span><span class="sxs-lookup"><span data-stu-id="03871-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="03871-104">راجع لا يمكنك استرداد العناصر [المحذوفة](https://aka.ms/pfrec)من مجلد عمومي غير بريد في Outlook 2016 .</span><span class="sxs-lookup"><span data-stu-id="03871-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="03871-105">**لاستعادة مجلد عمومي محذوف (من أي نوع)**:</span><span class="sxs-lookup"><span data-stu-id="03871-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="03871-106">الرجاء استخدام الأمر EXO PowerShell التالي:</span><span class="sxs-lookup"><span data-stu-id="03871-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="03871-107">بناء الجملة:</span><span class="sxs-lookup"><span data-stu-id="03871-107">Syntax:</span></span>

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    <span data-ttu-id="03871-108">مثال: سيستعيد الأمر التالي "المستعرض الفرعي1" ثم ضعه ضمن \Parent1:</span><span class="sxs-lookup"><span data-stu-id="03871-108">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

<span data-ttu-id="03871-109">راجع [استعادة مجلد عمومي محذوف](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) للحصول على مزيد من التفاصيل.</span><span class="sxs-lookup"><span data-stu-id="03871-109">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
