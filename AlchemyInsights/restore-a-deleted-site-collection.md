---
title: استعادة موقع محذوف
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: d37fd903c91c8cd6ac6137e815cb253f7edb4494
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/27/2020
ms.locfileid: "43912662"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="b70f4-102">استعادة موقع محذوف</span><span class="sxs-lookup"><span data-stu-id="b70f4-102">Restore a deleted site</span></span>

<span data-ttu-id="b70f4-103">عندما يحذف مسؤول موقع SharePoint، يتم وضعه في مجموعة سلة المهملات للموقع، حيث يتم الاحتفاظ به لمدة 93 يومًا قبل حذفه نهائيًا.</span><span class="sxs-lookup"><span data-stu-id="b70f4-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="b70f4-104">لاستعادة الموقع:</span><span class="sxs-lookup"><span data-stu-id="b70f4-104">To restore the site:</span></span>
  
1. <span data-ttu-id="b70f4-105">في مركز مسؤول SharePoint الجديد، انقر فوق **إعادة تدوير سلة المهملات** على الشريط.</span><span class="sxs-lookup"><span data-stu-id="b70f4-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="b70f4-106">حدد خانة الاختيار بجوار مجموعة الموقع التي تريد استعادتها.</span><span class="sxs-lookup"><span data-stu-id="b70f4-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="b70f4-107">انقر فوق **استعادة العناصر المحذوفة**.</span><span class="sxs-lookup"><span data-stu-id="b70f4-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="b70f4-108">لاستعادة موقع اتصال محذوف، يمكنك استخدام مركز مسؤول SharePoint الجديد.</span><span class="sxs-lookup"><span data-stu-id="b70f4-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="b70f4-109">وإلا، تحتاج إلى استخدام Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b70f4-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="b70f4-110">لاستعادة موقع ينتمي إلى مجموعة Microsoft 365، تحتاج إلى استعادة المجموعة في مركز إدارة Exchange.</span><span class="sxs-lookup"><span data-stu-id="b70f4-110">To restore a site that belongs to an Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="b70f4-111">يمكن استعادة المجموعات لمدة 30 يومًا بعد حذفها.</span><span class="sxs-lookup"><span data-stu-id="b70f4-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

