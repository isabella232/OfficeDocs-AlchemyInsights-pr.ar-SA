---
title: مزامنة ملف التعريف
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a841db70c238bdae58edfca634fe49a04ddce78a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320696"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>متى تتم مزامنة تغييرات ملف التعريف إلى SharePoint ملف تعريف المستخدم؟

SharePoint يستخدم Online مهمة "استيراد وقت Active Directory" (استيراد AD) لاستيراد المستخدمين والمجموعات إلى تطبيق ملف تعريف المستخدم. 
  
1. يقوم استيراد AD بمزامنة التغييرات من SharePoint Online Directory إلى تطبيق ملف تعريف المستخدم. تتم معالجة هذه التغييرات على دفعات.
    
2. يتم تشغيل مهمة الوقت حتى تتم مزامنة التغييرات.
    
**ملاحظة:** يتوقف الوقت الذي يستغرقه تشغيل المهمة على عدد التغييرات التي يجب إجراءها. يستغرق عدد كبير من التغييرات وقتا أطول. تظهر اتفاقية مستوى الخدمة (SLA) التغيير الذي تم إدخاله على مستخدم في SharePoint Online Directory في تطبيق ملف تعريف المستخدم في غضون 24 ساعة. 
  
[مزيد من المعلومات حول مزامنة ملف تعريف المستخدم في SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

