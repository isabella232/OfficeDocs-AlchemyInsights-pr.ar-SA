---
title: مزامنة ملف التعريف
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/18/2019
ms.locfileid: "36554320"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>عند تغيير ملف التعريف الخاص بي المزامنة إلى تطبيق التشكيل الجانبي للمستخدم SharePoint ؟

يستخدم SharePoint علي الإنترنت مهمة مؤقت "استيراد الدليل النشط" (استيراد AD) لاستيراد المستخدمين والمجموعات في "تطبيق ملف تعريف المستخدم". 
  
1. استيراد AD مزامنة التغييرات من مخزن دليل SharePoint علي الإنترنت إلى "تطبيق ملف تعريف المستخدم". تتم معالجه هذه التغييرات في دفعات.
    
2. يتم تشغيل مهمة المؤقت حتى تتم مزامنة التغييرات.
    
> [!NOTE]
> يعتمد الوقت المستغرق في تشغيل المهمة علي عدد التغييرات التي تتم علي العملية. عدد كبير من التغييرات يستغرق وقتا أطول. تنص اتفاقيه مستوي الخدمة (SLA) علي ان تغيير المستخدم في دليل SharePoint علي الإنترنت سينعكس في "تطبيق ملف تعريف المستخدم" في 24 ساعة. 
  
[مزيد من المعلومات حول مزامنة ملف تعريف المستخدم في SharePoint علي الإنترنت](https://go.microsoft.com/fwlink/?linkid=875671)
  

