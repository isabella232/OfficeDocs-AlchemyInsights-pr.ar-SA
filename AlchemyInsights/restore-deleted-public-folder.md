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
# <a name="restore-a-deleted-public-folder"></a>استعادة مجلد عمومي محذوف

**لاستعادة العناصر المحذوفة من مجلد عمومي:**

- راجع لا يمكنك استرداد العناصر [المحذوفة](https://aka.ms/pfrec)من مجلد عمومي غير بريد في Outlook 2016 .
 
**لاستعادة مجلد عمومي محذوف (من أي نوع)**: 

- الرجاء استخدام الأمر EXO PowerShell التالي:

    بناء الجملة:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    مثال: سيستعيد الأمر التالي "المستعرض الفرعي1" ثم ضعه ضمن \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

راجع [استعادة مجلد عمومي محذوف](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) للحصول على مزيد من التفاصيل.
