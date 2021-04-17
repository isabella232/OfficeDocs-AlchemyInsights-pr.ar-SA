---
title: سلوك التناسقGuid / sourceAnchor
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
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816979"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>سلوك التناسقGuid / sourceAnchor

يسهل Azure AD Connect (الإصدار 1.1.524.0 وما بعده) الآن استخدام msDS-ConsistencyGuid ك سمة sourceAnchor. عند استخدام هذه الميزة، يقوم Azure AD Connect تلقائيا بتكوين قواعد المزامنة من أجل:
  
- استخدم msDS-ConsistencyGuid ك السمة sourceAnchor كائنات المستخدم. يتم استخدام ObjectGUID لأنواع الكائنات الأخرى.
    
- بالنسبة لأي كائن مستخدم AD موقعي معين لم يتم ملء سمة msDS-ConsistencyGuid الخاصة به، يقوم Azure AD Connect بكتابة قيمة كائنGUID الخاصة به مرة أخرى إلى السمة msDS-ConsistencyGuid في Active Directory في الموقع. بعد تعبئة السمة msDS-ConsistencyGuid، يصدر Azure AD Connect الكائن إلى Azure AD.
    
 **ملاحظة:** بمجرد استيراد كائن AD المحلي إلى Azure AD Connect (أي، استيراده إلى "مساحة موصل AD" والتوقع إلى Metaverse)، لا يمكنك تغيير قيمة sourceAnchor الخاصة به بعد الآن. لتحديد قيمة sourceAnchor لكائن AD معين في الموقع، قم بتكوين السمة msDS-ConsistencyGuid قبل استيرادها إلى Azure AD Connect. 
  
لمزيد من المعلومات حول SourceAnchor وتناسقGuid، راجع ما [يلي: Azure AD Connect: مفاهيم التصميم](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

