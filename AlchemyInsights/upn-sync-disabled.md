---
title: تم تعطيل مزامنة UPN
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749501"
---
# <a name="upn-sync-disabled"></a>تم تعطيل مزامنة UPN

إذا بدات بالمزامنة إلى Azure AD قبل 30 مارس 2016 ، فقم بتشغيل الأمر Azure AD PowerShell cmdlet التالي لتمكين التطابق الضعيف لمؤسسك فقط:
  
 **مسولديرسينكفيتوري-ميزه انابليسوفتماتشونوبن-تمكين ال$True**
  
يتم تشغيل التطابق الفعال ل UPN تلقائيا للمؤسسات التي بدات المزامنة في Azure AD أو بعد 30 مارس 2016.
  
لمعرفه المزيد حول تمكين التطابق البسيط علي UPN وميزات المزامنة الأخرى ، يرجى مراجعه [ميزات خدمه مزامنة AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

