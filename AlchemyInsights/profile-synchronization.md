---
title: مزامنة ملف التعريف
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a32cf9e623d1be7a2c85ef4951c6eb7f001b7db0
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/24/2019
ms.locfileid: "29456304"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="bc7d7-102">لتطبيق ملف تعريف المستخدم SharePoint عند مزامنة التغييرات الشخصية الخاصة بي؟</span><span class="sxs-lookup"><span data-stu-id="bc7d7-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="bc7d7-103">يستخدم SharePoint على الإنترنت مهمة مؤقت "استيراد الدليل النشط" (استيراد AD) لاستيراد مستخدمين ومجموعات إلى "تطبيق ملف تعريف المستخدم".</span><span class="sxs-lookup"><span data-stu-id="bc7d7-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="bc7d7-p101">استيراد AD مزامنة التغييرات من المتجر على إنترنت دليل SharePoint "تطبيق ملف تعريف المستخدم". تتم معالجة هذه التغييرات على دفعات.</span><span class="sxs-lookup"><span data-stu-id="bc7d7-p101">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application. These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="bc7d7-106">تشغيل مهمة مؤقت حتى تتم مزامنة التغييرات.</span><span class="sxs-lookup"><span data-stu-id="bc7d7-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="bc7d7-p102">يعتمد الوقت المستغرق لتشغيل الوظيفة على عدد التغييرات لمعالجة. عدد كبير من التغييرات وقتاً أطول. تنص اتفاقية مستوى الخدمة (SLA) أن تغيير لمستخدم في دليل الإنترنت SharePoint تنعكس في "تطبيق ملف تعريف المستخدم" في غضون 24 ساعة.</span><span class="sxs-lookup"><span data-stu-id="bc7d7-p102">The time it takes the job to run depends on the number of changes to process. A large number of changes takes longer. The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="bc7d7-110">مزيد من المعلومات حول مزامنة ملف تعريف المستخدم في SharePoint عبر إنترنت</span><span class="sxs-lookup"><span data-stu-id="bc7d7-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

