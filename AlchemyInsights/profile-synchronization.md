---
title: مزامنة ملف التعريف
ms.author: arnek
author: arnek
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: dc6e0280961d14aa3e6bd466afbe0cbe89418d17
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43768100"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="67ad6-102">متى تتم مزامنة ملف التعريف الخاص بي مع تطبيق ملف تعريف المستخدم SharePoint؟</span><span class="sxs-lookup"><span data-stu-id="67ad6-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="67ad6-103">يستخدم SharePoint Online مهمة مؤقت استيراد الدليل النشط (استيراد الإعلانية) لاستيراد المستخدمين والمجموعات إلى تطبيق ملف تعريف المستخدم.</span><span class="sxs-lookup"><span data-stu-id="67ad6-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="67ad6-104">يقوم استيراد الإعلانية بمزامنة التغييرات من مخزن الدليل عبر الإنترنت SharePoint إلى تطبيق ملف تعريف المستخدم.</span><span class="sxs-lookup"><span data-stu-id="67ad6-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="67ad6-105">تتم معالجة هذه التغييرات على دفعات.</span><span class="sxs-lookup"><span data-stu-id="67ad6-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="67ad6-106">يتم تشغيل مهمة المؤقت حتى تتم مزامنة التغييرات.</span><span class="sxs-lookup"><span data-stu-id="67ad6-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="67ad6-107">يعتمد الوقت الذي تستغرقه المهمة لتشغيلها على عدد التغييرات التي يجب معالجتها.</span><span class="sxs-lookup"><span data-stu-id="67ad6-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="67ad6-108">يستغرق عدد كبير من التغييرات وقتًا أطول.</span><span class="sxs-lookup"><span data-stu-id="67ad6-108">A large number of changes takes longer.</span></span> <span data-ttu-id="67ad6-109">تنص اتفاقية مستوى الخدمة (SLA) على أن التغيير إلى مستخدم في دليل SharePoint عبر الإنترنت سينعكس في تطبيق ملف تعريف المستخدم في 24 ساعة.</span><span class="sxs-lookup"><span data-stu-id="67ad6-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="67ad6-110">مزيد من المعلومات حول مزامنة ملف تعريف المستخدم في SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="67ad6-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

