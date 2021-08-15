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
ms.openlocfilehash: fc163fae4d348d7c7cf117bd457f999b42f96bec7c1eb9aa1435e346131d06de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038099"
---
# <a name="upn-sync-disabled"></a>تم تعطيل مزامنة UPN

إذا بدأت المزامنة إلى Azure AD قبل 30 مارس 2016، ف قم بتشغيل الأمر cmdlet التالي ل Azure AD PowerShell لتمكين مطابقة UPN الناعمة لم المؤسسة فقط:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
يتم تشغيل مطابقة UPN الناعمة تلقائيا في المؤسسات التي بدأت المزامنة إلى Azure AD في 30 مارس 2016 أو بعده.
  
لمعرفة المزيد حول تمكين المزامنة الناعمة على UPN وميزات المزامنة الأخرى، الرجاء الاطلاع على [Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)الاتصال ميزات خدمة المزامنة .
  

