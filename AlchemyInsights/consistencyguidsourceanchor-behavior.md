---
title: سلوك كونسيستينسيجويد/سورسيانتشور
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
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: adac469328485696d1ee1532aa3d6828af0642eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756270"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>سلوك كونسيستينسيجويد/سورسينتشور

يسهل الآن Azure AD Connect (الإصدار 1.1.524.0 وما يليه) استخدام السمة مسدس-كونسيستينسيجويد كسورسينتشور. عند استخدام هذه الميزة ، يقوم Azure AD بتكوين قواعد المزامنة تلقائيا إلى:
  
- استخدم مسدس-كونسيستينسيجويد كسمه سورسينتشور لكائنات المستخدم. يتم استخدام أوبجيكتجويد لأنواع الكائنات الأخرى.
    
- بالنسبة إلى اي كائن المستخدم المحلي الخاص بالإعلانات المحددة التي لا يتم تعبئة السمة مسدس الخاصة بها ، فان Azure AD Connect تكتب قيمه أوبجيكتجويد الخاصة بها مره أخرى إلى السمة مسدس-كونسيستينسيجويد في Active Directory المحلي. بعد تعبئة السمة مسدس-كونسيستينسيجويد ، يقوم Azure AD Connect بتصدير الكائن إلى Azure AD.
    
 **ملاحظه:** بمجرد استيراد كائن الإعلانات المحلي إلى Azure AD Connect (والذي يتم استيراده إلى مساحة موصل الإعلانات وعرضه في ميتافيرسي) ، لا يمكنك تغيير قيمه سورسيانتشور الخاصة به. لتحديد القيمة سورسيانتشور لكائن إعلانات معين في الموقع المحلي ، قم بتكوين سمه مسدس-كونسيستينسيجويد قبل استيرادها إلى Azure AD Connect. 
  
للحصول علي مزيد من المعلومات حول سورسينتشور و كونسيستينسيجويد ، يمكنك الرجوع إلى ما يلي: [AZURE AD Connect: مفاهيم التصميم](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

