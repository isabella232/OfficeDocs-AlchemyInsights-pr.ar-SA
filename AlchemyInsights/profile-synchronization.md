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
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="485e4-102">عند تغيير ملف التعريف الخاص بي المزامنة إلى تطبيق التشكيل الجانبي للمستخدم SharePoint ؟</span><span class="sxs-lookup"><span data-stu-id="485e4-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="485e4-103">يستخدم SharePoint علي الإنترنت مهمة مؤقت "استيراد الدليل النشط" (استيراد AD) لاستيراد المستخدمين والمجموعات في "تطبيق ملف تعريف المستخدم".</span><span class="sxs-lookup"><span data-stu-id="485e4-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="485e4-104">استيراد AD مزامنة التغييرات من مخزن دليل SharePoint علي الإنترنت إلى "تطبيق ملف تعريف المستخدم".</span><span class="sxs-lookup"><span data-stu-id="485e4-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="485e4-105">تتم معالجه هذه التغييرات في دفعات.</span><span class="sxs-lookup"><span data-stu-id="485e4-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="485e4-106">يتم تشغيل مهمة المؤقت حتى تتم مزامنة التغييرات.</span><span class="sxs-lookup"><span data-stu-id="485e4-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="485e4-107">يعتمد الوقت المستغرق في تشغيل المهمة علي عدد التغييرات التي تتم علي العملية.</span><span class="sxs-lookup"><span data-stu-id="485e4-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="485e4-108">عدد كبير من التغييرات يستغرق وقتا أطول.</span><span class="sxs-lookup"><span data-stu-id="485e4-108">A large number of changes takes longer.</span></span> <span data-ttu-id="485e4-109">تنص اتفاقيه مستوي الخدمة (SLA) علي ان تغيير المستخدم في دليل SharePoint علي الإنترنت سينعكس في "تطبيق ملف تعريف المستخدم" في 24 ساعة.</span><span class="sxs-lookup"><span data-stu-id="485e4-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="485e4-110">مزيد من المعلومات حول مزامنة ملف تعريف المستخدم في SharePoint علي الإنترنت</span><span class="sxs-lookup"><span data-stu-id="485e4-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

