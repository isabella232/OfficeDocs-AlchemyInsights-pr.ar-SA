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
ms.openlocfilehash: 4243cdf0170fed1eadac6560d2a04e1a861c63e5
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2020
ms.locfileid: "42043563"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>لدفعة ترحيل المجلد العمومي مع حالة CompleteedWithErrors

استخدم الخطوات التالية لإكمال الدفعة، تخطي العناصر الكبيرة/السيئة: 
1. الموافقة على العناصر التي تم تخطيها في دفعة الترحيل:

    تعيين ترحيلBatch \<اسم الدفعة> -ApproveSkipedItems 
2. استخدم الأمر التالي للموافقة على العناصر التي تم تخطيها في طلبات الترحيل التي تمت "مزامنتها" ولكن لم تكتمل:

    $pf = Get-PublicFolderMailboxMigrationRequest | الحصول على PublicFolderMailboxMigrationRequestStatistics -تضمينالتقرير; ForEach ($i في $pf) {إذا ($i.LargeItemsEncountered -gt 0 -أو $i.BadItemsEncountered -gt 0) {Set-publicFolderMailboxRequestrequest $i.Identity.IdentifyingGuid -SkipedItemApprovalTime $([DateTime]::UtcNow)}}
3. يجب استئناف دفعة الترحيل والطلبات وإكمالها في بضع دقائق.

