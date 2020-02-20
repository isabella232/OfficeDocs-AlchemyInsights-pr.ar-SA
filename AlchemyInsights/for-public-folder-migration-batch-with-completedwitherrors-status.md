---
title: لدفعة ترحيل المجلد العمومي مع حالة CompleteedWithErrors
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
- "3532"
ms.openlocfilehash: 739e9d91f90e4c0374814d199e4372eb5625553a
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158584"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>لدفعة ترحيل المجلد العمومي مع حالة CompleteedWithErrors

استخدم الخطوات التالية لإكمال الدفعة، تخطي العناصر الكبيرة/السيئة: 
1. الموافقة على العناصر التي تم تخطيها في دفعة الترحيل:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. استخدم الأمر التالي للموافقة على العناصر التي تم تخطيها في طلبات الترحيل التي تمت "مزامنتها" ولكن لم تكتمل:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. يجب استئناف دفعة الترحيل والطلبات وإكمالها في بضع دقائق.

