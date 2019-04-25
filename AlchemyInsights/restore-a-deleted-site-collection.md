---
title: استعادة موقع المحذوفة
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 5/1/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 0cf10a3a0effc1774d8a07c5d0be96384362c175
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/23/2019
ms.locfileid: "32369809"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="9387d-102">استعادة موقع المحذوفة</span><span class="sxs-lookup"><span data-stu-id="9387d-102">Restore a deleted site</span></span>

<span data-ttu-id="9387d-103">عندما يقوم مسؤول حذف موقع، يتم وضعها في مجموعة موقع "سلة المحذوفات"، حيث تظل لأيام 93 قبل إلغائها نهائياً.</span><span class="sxs-lookup"><span data-stu-id="9387d-103">When an admin deletes a site , it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="9387d-104">لاستعادة الموقع:</span><span class="sxs-lookup"><span data-stu-id="9387d-104">To restore the site:</span></span>
  
1. <span data-ttu-id="9387d-105">في مركز مسؤول SharePoint جديد، انقر فوق **"سلة المحذوفات"** على "الشريط".</span><span class="sxs-lookup"><span data-stu-id="9387d-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="9387d-106">حدد خانة الاختيار المجاورة لمجموعة الموقع التي تريد استعادتها.</span><span class="sxs-lookup"><span data-stu-id="9387d-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="9387d-107">انقر فوق **استعادة العناصر المحذوفة**.</span><span class="sxs-lookup"><span data-stu-id="9387d-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="9387d-108">لاستعادة موقع اتصال محذوفة، يمكنك استخدام مركز مسؤول SharePoint جديدة.</span><span class="sxs-lookup"><span data-stu-id="9387d-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="9387d-109">وإلا، تحتاج إلى استخدام Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9387d-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="9387d-110">لاستعادة موقع الذي ينتمي إلى مجموعة Office 365، تحتاج إلى استعادة المجموعة في مركز مسؤول Exchange.</span><span class="sxs-lookup"><span data-stu-id="9387d-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="9387d-111">يمكن استعادة مجموعات لمدة 30 يوما بعد أن كنت حذفها.</span><span class="sxs-lookup"><span data-stu-id="9387d-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

