---
title: تم تعطيل مزامنة UPN
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2b1ba772459091ce1a796884997fe2516d0407eb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782138"
---
# <a name="upn-sync-disabled"></a>تم تعطيل مزامنة UPN

إذا بدأت المزامنة إلى Azure AD قبل 30 مارس 2016، ف قم بتشغيل الأمر cmdlet التالي ل Azure AD PowerShell لتمكين مطابقة UPN الناعمة لم المؤسسة فقط:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
يتم تشغيل مطابقة UPN الناعمة تلقائيا في المؤسسات التي بدأت المزامنة إلى Azure AD في 30 مارس 2016 أو بعده.
  
لمعرفة المزيد حول تمكين المزامنة الناعمة على UPN وميزات المزامنة الأخرى، الرجاء الاطلاع على [ميزات خدمة مزامنة Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

