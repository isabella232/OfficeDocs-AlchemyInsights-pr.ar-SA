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
# <a name="upn-sync-disabled"></a>تعطيل مزامنة UPN

إذا بدأت المزامنة مع Azure AD قبل 30 مارس 2016، قم بتشغيل cmdlet Azure AD PowerShell التالية لتمكين مطابقة UPN الناعمة لمؤسستك فقط:
  
 **تعيين-MsoldirSyncFeature -ميزة EnableSoftMatchOnUpn -تمكين $True**
  
يتم تشغيل المطابقة الناعمة لـ UPN تلقائيًا للمؤسسات التي بدأت المزامنة مع Azure AD في 30 مارس 2016 أو بعده.
  
لمعرفة المزيد حول تمكين المطابقة الناعمة على UPN وميزات المزامنة الأخرى، يرجى الاطلاع على [ميزات خدمة مزامنة Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

