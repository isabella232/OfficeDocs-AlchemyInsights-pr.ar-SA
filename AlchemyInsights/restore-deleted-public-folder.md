---
title: استعاده مجلد عمومي محذوف
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
- "3488"
ms.openlocfilehash: bb7fe248714e9a7e7f4c48913b159b5c23132192
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774518"
---
# <a name="restore-a-deleted-public-folder"></a>استعاده مجلد عمومي محذوف

**لاستعاده العناصر المحذوفة من مجلد عمومي**:

- راجع [لا يمكنك استرداد العناصر المحذوفة من مجلد البريد الكتروني غير البريدي في Outlook 2016](https://aka.ms/pfrec).
 
**لاستعاده مجلد عمومي محذوف (من اي نوع)**: 

- يرجى استخدام الأمر أكسو PowerShell التالي:

    بناء جمله

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    مثال: سيقوم الأمر التالي باستعادة Subfolder1 ووضعه ضمن \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

راجع [استعاده مجلد عمومي محذوف](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) للحصول علي مزيد من التفاصيل.
