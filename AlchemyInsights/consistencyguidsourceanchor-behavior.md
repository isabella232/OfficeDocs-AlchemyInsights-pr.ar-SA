---
title: السلوك المتناسق/الدليل المرجعي
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: f0ff94a8e46f1fb4e0ac8653c51f8f651e29498b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/18/2019
ms.locfileid: "36516951"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>السلوك المتناسق/الدليل المرجعي

الإعلان Azure الاتصال (الإصدار 1.1.524.0 وبعد) الآن يسهل استخدام السمة الخاصة بالاسم الثابت. عند استخدام هذه الميزة الاتصال AD Azure تلقائيا بتكوين قواعد المزامنة إلى:
  
- استخدام الخصائص الثابتة كسمه المرجع لكائنات المستخدم. يتم استخدام ObjectGUID لأنواع الكائنات الأخرى.
    
- بالنسبة لأي كائن المستخدم AD المحلية التي لا يتم تعبئة السمة الخاصة به التي لا يتم نشرها ، Azure AD الاتصال يكتب القيمة objectGUID الخاصة به إلى السمة-المنطقية القوية في "Active Directory" المحلي. بعد ان يتم تعبئة السمة-التناسق الذي تم ملؤه ، أزور الإعلان الاتصال ثم تصدير الكائن إلى AD Azure.
    
 **ملاحظه:** بمجرد استيراد كائن AD داخلي إلى الاتصال AD Azure (اي ، استيراد إلى مساحة موصل AD والمتوقعة في Metaverse) ، لا يمكنك تغيير قيمه الدليل الخاص به بعد الآن. لتحديد قيمه المرجع لكائن AD داخلي معين ، قم بتكوين السمة الخاصة به الخاصة بالمسدسات المنطقية قبل استيرادها إلى اتصال AD Azure. 
  
لمزيد من المعلومات حول المرجع والتناسق ، راجع ما يلي: [الاتصال الإعلان Azure: مفاهيم التصميم](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

