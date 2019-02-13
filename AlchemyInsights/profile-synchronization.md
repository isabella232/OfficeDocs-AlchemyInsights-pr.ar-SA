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
ms.openlocfilehash: d1a72a85767e36fefbfa8eee266befcaf2e48af0
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29920075"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="a48e3-102">لتطبيق ملف تعريف المستخدم SharePoint عند مزامنة التغييرات الشخصية الخاصة بي؟</span><span class="sxs-lookup"><span data-stu-id="a48e3-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="a48e3-103">يستخدم SharePoint على الإنترنت مهمة مؤقت "استيراد الدليل النشط" (استيراد AD) لاستيراد مستخدمين ومجموعات إلى "تطبيق ملف تعريف المستخدم".</span><span class="sxs-lookup"><span data-stu-id="a48e3-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="a48e3-p101">استيراد AD مزامنة التغييرات من المتجر على إنترنت دليل SharePoint "تطبيق ملف تعريف المستخدم". تتم معالجة هذه التغييرات على دفعات.</span><span class="sxs-lookup"><span data-stu-id="a48e3-p101">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application. These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="a48e3-106">تشغيل مهمة مؤقت حتى تتم مزامنة التغييرات.</span><span class="sxs-lookup"><span data-stu-id="a48e3-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="a48e3-p102">يعتمد الوقت المستغرق لتشغيل الوظيفة على عدد التغييرات لمعالجة. عدد كبير من التغييرات وقتاً أطول. تنص اتفاقية مستوى الخدمة (SLA) أن تغيير لمستخدم في دليل الإنترنت SharePoint تنعكس في "تطبيق ملف تعريف المستخدم" في غضون 24 ساعة.</span><span class="sxs-lookup"><span data-stu-id="a48e3-p102">The time it takes the job to run depends on the number of changes to process. A large number of changes takes longer. The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="a48e3-110">مزيد من المعلومات حول مزامنة ملف تعريف المستخدم في SharePoint عبر إنترنت</span><span class="sxs-lookup"><span data-stu-id="a48e3-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

