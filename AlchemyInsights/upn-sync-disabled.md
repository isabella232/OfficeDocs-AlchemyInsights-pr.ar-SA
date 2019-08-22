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
ms.openlocfilehash: f390d659b191fa4c44bd7c8acb32409cd3021489
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36532318"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="392de-102">تعطيل المزامنة UPN</span><span class="sxs-lookup"><span data-stu-id="392de-102">UPN sync disabled</span></span>

<span data-ttu-id="392de-103">إذا قمت ببدء تشغيل المزامنة لإعلان Azure قبل 30 آذار/مارس 2016، قم بتشغيل cmdlet PowerShell الإعلان Azure التالية لتمكين مطابقة UPN ناعمة للمؤسسة الخاصة بك فقط:</span><span class="sxs-lookup"><span data-stu-id="392de-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="392de-104">**مجموعة مسولديرسينكفيتوري-تتميز انابليسوفتماتشونوبن-تمكين $True**</span><span class="sxs-lookup"><span data-stu-id="392de-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="392de-105">مطابقة ناعمة UPN قيد التشغيل تلقائياً للمؤسسات بدء المزامنة لإعلان الﻻزوردية في أو بعد 30 مارس عام 2016.</span><span class="sxs-lookup"><span data-stu-id="392de-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="392de-106">لمعرفة المزيد حول تمكين مطابقة الناعمة على UPN وميزات المزامنة، راجع [ميزات خدمة المزامنة الاتصال الإعلان Azure](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="392de-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

