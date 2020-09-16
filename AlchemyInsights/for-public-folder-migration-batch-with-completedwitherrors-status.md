---
title: بالنسبة إلى دفعه الترحيل للمجلد العام مع حاله كومبليتيدويثيرورس
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
- "3532"
ms.openlocfilehash: cbf5237fdb5c660057465e67702e35f68e545ddb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744100"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>بالنسبة إلى دفعه الترحيل للمجلد العام مع حاله كومبليتيدويثيرورس

استخدم الخطوات التالية لإكمال الدفعة ، مع تخطي العناصر الكبيرة/غير الصالحة: 
1. الموافقة علي العناصر المتخطاه علي دفعه الترحيل:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. استخدم الأمر التالي للموافقة علي العناصر المتخطاه علي طلبات الترحيل التي تمت مزامنتها ، ولكن لم يتم إكمالها:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. يجب استئناف دفعه الترحيل والطلبات وإكمالها خلال دقائق قليله.

