---
title: تعطيل المزامنة UPN
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2a03ac64d92c07b523b015850251b33c58bb76f8
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/22/2019
ms.locfileid: "30767200"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="486cb-102">تعطيل المزامنة UPN</span><span class="sxs-lookup"><span data-stu-id="486cb-102">UPN sync disabled</span></span>

<span data-ttu-id="486cb-103">إذا قمت ببدء تشغيل المزامنة لإعلان Azure قبل 30 آذار/مارس 2016، قم بتشغيل cmdlet PowerShell الإعلان Azure التالية لتمكين مطابقة UPN ناعمة للمؤسسة الخاصة بك فقط:</span><span class="sxs-lookup"><span data-stu-id="486cb-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="486cb-104">**مجموعة مسولديرسينكفيتوري-تتميز انابليسوفتماتشونوبن-تمكين $True**</span><span class="sxs-lookup"><span data-stu-id="486cb-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="486cb-105">مطابقة ناعمة UPN قيد التشغيل تلقائياً للمؤسسات بدء المزامنة لإعلان الﻻزوردية في أو بعد 30 مارس عام 2016.</span><span class="sxs-lookup"><span data-stu-id="486cb-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="486cb-106">لمعرفة المزيد حول تمكين مطابقة الناعمة على UPN وميزات المزامنة، راجع [ميزات خدمة المزامنة الاتصال الإعلان Azure](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="486cb-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

