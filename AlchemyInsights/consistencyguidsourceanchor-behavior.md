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
ms.openlocfilehash: 9b5765ff3c59b1312bead41a45a53478a96260df0567f006ab93c3ccfaf4be64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044327"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>سلوك التناسقGuid / sourceAnchor

يسهل Azure AD الاتصال (الإصدار 1.1.524.0 وما بعده) الآن استخدام msDS-ConsistencyGuid ك سمة sourceAnchor. عند استخدام هذه الميزة، يقوم Azure AD الاتصال تلقائيا بتكوين قواعد المزامنة من أجل:
  
- استخدم msDS-ConsistencyGuid ك السمة sourceAnchor كائنات المستخدم. يتم استخدام ObjectGUID لأنواع الكائنات الأخرى.
    
- بالنسبة لأي كائن مستخدم AD موقعي معين لم يتم ملء سمة msDS-ConsistencyGuid الخاصة به، يقوم Azure AD الاتصال بكتابة قيمة كائنGUID الخاصة به مرة أخرى إلى السمة msDS-ConsistencyGuid في Active Directory في الموقع. بعد تعبئة السمة msDS-ConsistencyGuid، الاتصال Azure AD بعد ذلك تصدير الكائن إلى Azure AD.
    
 **ملاحظة:** بعد استيراد كائن AD المحلي إلى Azure AD الاتصال (أي، استيراده إلى "مساحة موصل AD" والتوقع إلى Metaverse)، لا يمكنك تغيير قيمة sourceAnchor الخاصة به بعد الآن. لتحديد قيمة sourceAnchor لكائن AD معين في الموقع، قم بتكوين السمة msDS-ConsistencyGuid قبل استيرادها إلى Azure AD الاتصال. 
  
لمزيد من المعلومات حول SourceAnchor وتناسقGuid، راجع ما [يلي: Azure AD الاتصال: مفاهيم التصميم](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

