---
title: كونسيستينسيجويد/سورسينتشور السلوك
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: e1ffa9cf2b59570cb6ea3517efad7a55fd9489a8
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29927604"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>كونسيستينسيجويد/سورسينتشور السلوك

الاتصال الإعلان أزور (الإصدار 1.1.524.0 وبعد) يسهل استخدام مسدس كونسيستينسيجويد كسمة سورسينتشور الآن. عند استخدام هذه الميزة، Azure الإعلان الاتصال تلقائياً بتكوين قواعد المزامنة إلى:
  
- استخدام مسدس كونسيستينسيجويد كسمة سورسينتشور لكائنات المستخدم. يتم استخدام دليل الكائن لأنواع الكائنات الأخرى.
    
- لأي إعطاء الداخلي المستخدم الإعلان الكائن الذي سمته مسدس كونسيستينسيجويد لا يكتب الاتصال الإعلان المعممة، Azure قيمته دليل الكائن مرة أخرى إلى سمة كونسيستينسيجويد مسدس في "Active Directory" على أماكن العمل. بعد أن يتم نشر السمة كونسيستينسيجويد مسدس أو الاتصال الإعلان Azure ثم يصدر الكائن لإعلان Azure.
    
 **ملاحظة:** مرة داخلي استيراد كائن الإعلان إلى Azure الإعلان الاتصال (أي، المستوردة إلى "مساحة موصل" الإعلان والمرتقب في Metaverse)، لا يمكن تغيير قيمته سورسيانتشور بعد الآن. لتعيين القيمة سورسينتشور للداخلي نظراً لإعلان الكائن، قم بتكوين سمة كونسيستينسيجويد مسدس به قبل استيرادها إلى الاتصال الإعلان Azure. 
  
لمزيد من المعلومات حول سورسينتشور وكونسيستينسيجويد، أرجع إلى ما يلي: [أزور الاتصال الإعلان: مفاهيم التصميم](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

