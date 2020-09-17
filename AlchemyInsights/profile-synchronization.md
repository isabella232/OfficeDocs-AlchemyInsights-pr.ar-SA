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
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="79a5f-102">متى يتم مزامنة تغييرات التشكيل الجانبي إلى تطبيق ملف تعريف المستخدم في SharePoint ؟</span><span class="sxs-lookup"><span data-stu-id="79a5f-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="79a5f-103">يستخدم SharePoint Online مهمة مؤقت استيراد Active directory (استيراد AD) لاستيراد المستخدمين والمجموعات إلى تطبيق ملف تعريف المستخدم.</span><span class="sxs-lookup"><span data-stu-id="79a5f-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="79a5f-104">يقوم "استيراد الإعلانات" بمزامنة التغييرات من مخزن دليل SharePoint Online إلى تطبيق ملف تعريف المستخدم.</span><span class="sxs-lookup"><span data-stu-id="79a5f-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="79a5f-105">تتم معالجه هذه التغييرات في الدفعات.</span><span class="sxs-lookup"><span data-stu-id="79a5f-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="79a5f-106">يتم تشغيل مهمة المؤقت حتى تتم مزامنة التغييرات.</span><span class="sxs-lookup"><span data-stu-id="79a5f-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="79a5f-107">تعتمد المدة التي يستغرقها تشغيل المهمة علي عدد التغييرات التي يجب معالجتها.</span><span class="sxs-lookup"><span data-stu-id="79a5f-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="79a5f-108">تستغرق عدد كبير من التغييرات وقتا أطول.</span><span class="sxs-lookup"><span data-stu-id="79a5f-108">A large number of changes takes longer.</span></span> <span data-ttu-id="79a5f-109">الاتفاقية علي مستوي الخدمة (SLA) تنص علي انه سيتم عكس تغيير المستخدم في دليل SharePoint Online في تطبيق ملف تعريف المستخدم خلال 24 ساعة.</span><span class="sxs-lookup"><span data-stu-id="79a5f-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="79a5f-110">مزيد من المعلومات حول مزامنة ملف تعريف المستخدم في SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="79a5f-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

