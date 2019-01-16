---
title: تعطيل المزامنة UPN
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: d00f10688ec775c22d60a9089e291c265ada46f1
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/15/2019
ms.locfileid: "28273977"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="74412-102">تعطيل المزامنة UPN</span><span class="sxs-lookup"><span data-stu-id="74412-102">UPN sync disabled</span></span>

<span data-ttu-id="74412-103">إذا قمت ببدء تشغيل المزامنة لإعلان Azure قبل 30 آذار/مارس 2016، قم بتشغيل cmdlet PowerShell الإعلان Azure التالية لتمكين مطابقة UPN ناعمة للمؤسسة الخاصة بك فقط:</span><span class="sxs-lookup"><span data-stu-id="74412-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="74412-104">**مجموعة مسولديرسينكفيتوري-تتميز انابليسوفتماتشونوبن-تمكين $True**</span><span class="sxs-lookup"><span data-stu-id="74412-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="74412-105">مطابقة ناعمة UPN قيد التشغيل تلقائياً للمؤسسات بدء المزامنة لإعلان الﻻزوردية في أو بعد 30 مارس عام 2016.</span><span class="sxs-lookup"><span data-stu-id="74412-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="74412-106">لمعرفة المزيد حول تمكين مطابقة الناعمة على UPN وميزات المزامنة، راجع [ميزات خدمة المزامنة الاتصال الإعلان Azure](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="74412-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

