---
title: تمكين تدقيق علبة البريد
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
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: ae11d6be0789a5662d202b85268480a3d42922c4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703558"
---
# <a name="enable-mailbox-auditing"></a>تمكين تدقيق علبة البريد

لتمكين تدقيق علبة البريد لمستخدم واحد أو مؤسسة بأكملها يجب تشغيل cmdlets التالية من شل الطاقة البعيد:
  
 **مستخدم واحد**
  
مجموعة علبة البريد - الهوية "جين داو" -AuditEnabled $true
  
 **المنظمه**
  
الحصول على علبة البريد -ResultSize غير محدود -تصفية {RecipientTypeDetails-eq "UserMailbox"} | $true مجموعة علبة البريد -AuditEnabled
  
[التعرف على المزيد](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

