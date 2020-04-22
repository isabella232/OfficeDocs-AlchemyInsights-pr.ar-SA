---
title: ConsistencyGuid / سلوك مرساة المصدر
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
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 8527e7c2404742a999041f85ed12d78c48cc0d8c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705720"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / سلوك مرساة المصدر

Azure AD Connect (الإصدار 1.1.524.0 وما بعده) يسهل الآن استخدام msDS-ConsistencyGuid كسمة sourceAnchor. عند استخدام هذه الميزة، يقوم Azure AD Connect بتكوين قواعد المزامنة تلقائيًا إلى:
  
- استخدم msDS-ConsistencyGuid كسمة sourceAnchor لكائنات المستخدم. يتم استخدام ObjectGUID لأنواع الكائنات الأخرى.
    
- لأي كائن مستخدم AD معين داخليًا لا يتم ملء سمة msDS-ConsistencyGuid الخاصة به، يقوم Azure AD Connect بكتابة قيمة objectGUID الخاصة به مرة أخرى إلى سمة msDS-ConsistencyGuid في الدليل النشط الداخلي. بعد ملء السمة msDS-ConsistencyGuid، يقوم Azure AD Connect بعد ذلك بتصدير الكائن إلى Azure AD.
    
 **ملاحظة:** بمجرد استيراد كائن AD داخلي إلى Azure AD Connect (أي استيراده إلى مساحة موصل الإعلانية والمتوقع في Metaverse)، لا يمكنك تغيير قيمة المصدر Anchor بعد الآن. لتحديد قيمة sourceAnchor لكائن AD داخلي معين، قم بتكوين سمة msDS-ConsistencyGuid قبل استيرادها إلى Azure AD Connect. 
  
لمزيد من المعلومات حول SourceAnchor وConsistencyGuid، راجع ما يلي: [Azure AD Connect: مفاهيم التصميم](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

