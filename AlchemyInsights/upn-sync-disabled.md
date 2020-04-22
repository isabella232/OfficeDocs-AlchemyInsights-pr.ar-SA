---
title: تعطيل مزامنة UPN
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 33bc7e30d41ff70e2ce55d946202acf45dbcb0f2
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726091"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="d443e-102">تعطيل مزامنة UPN</span><span class="sxs-lookup"><span data-stu-id="d443e-102">UPN sync disabled</span></span>

<span data-ttu-id="d443e-103">إذا بدأت المزامنة مع Azure AD قبل 30 مارس 2016، قم بتشغيل cmdlet Azure AD PowerShell التالية لتمكين مطابقة UPN الناعمة لمؤسستك فقط:</span><span class="sxs-lookup"><span data-stu-id="d443e-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="d443e-104">**تعيين-MsoldirSyncFeature -ميزة EnableSoftMatchOnUpn -تمكين $True**</span><span class="sxs-lookup"><span data-stu-id="d443e-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="d443e-105">يتم تشغيل المطابقة الناعمة لـ UPN تلقائيًا للمؤسسات التي بدأت المزامنة مع Azure AD في 30 مارس 2016 أو بعده.</span><span class="sxs-lookup"><span data-stu-id="d443e-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="d443e-106">لمعرفة المزيد حول تمكين المطابقة الناعمة على UPN وميزات المزامنة الأخرى، يرجى الاطلاع على [ميزات خدمة مزامنة Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="d443e-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

