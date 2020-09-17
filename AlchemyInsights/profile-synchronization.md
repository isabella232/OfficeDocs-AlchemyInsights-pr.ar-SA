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
ms.openlocfilehash: eee1080a95955332e205db3852381e39aaf5ae0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801756"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>متى يتم مزامنة تغييرات التشكيل الجانبي إلى تطبيق ملف تعريف المستخدم في SharePoint ؟

يستخدم SharePoint Online مهمة مؤقت استيراد Active directory (استيراد AD) لاستيراد المستخدمين والمجموعات إلى تطبيق ملف تعريف المستخدم. 
  
1. يقوم "استيراد الإعلانات" بمزامنة التغييرات من مخزن دليل SharePoint Online إلى تطبيق ملف تعريف المستخدم. تتم معالجه هذه التغييرات في الدفعات.
    
2. يتم تشغيل مهمة المؤقت حتى تتم مزامنة التغييرات.
    
> [!NOTE]
> تعتمد المدة التي يستغرقها تشغيل المهمة علي عدد التغييرات التي يجب معالجتها. تستغرق عدد كبير من التغييرات وقتا أطول. الاتفاقية علي مستوي الخدمة (SLA) تنص علي انه سيتم عكس تغيير المستخدم في دليل SharePoint Online في تطبيق ملف تعريف المستخدم خلال 24 ساعة. 
  
[مزيد من المعلومات حول مزامنة ملف تعريف المستخدم في SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

