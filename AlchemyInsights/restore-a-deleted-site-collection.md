---
title: استعاده موقع محذوف
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
ms.openlocfilehash: edf851da951e163f30660d524049abe0798a8314
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048783"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="de9c8-102">استعاده موقع محذوف</span><span class="sxs-lookup"><span data-stu-id="de9c8-102">Restore a deleted site</span></span>

<span data-ttu-id="de9c8-103">عندما يحذف أحد المسؤولين موقع SharePoint ، يتم وضعه في سله محذوفات مجموعه الموقع ، حيث يتم الاحتفاظ به لمده 93 يوما قبل حذفه نهائيا.</span><span class="sxs-lookup"><span data-stu-id="de9c8-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="de9c8-104">لاستعاده الموقع:</span><span class="sxs-lookup"><span data-stu-id="de9c8-104">To restore the site:</span></span>
  
1. <span data-ttu-id="de9c8-105">في مركز مسؤول SharePoint الجديد ، انقر فوق سله **المحذوفات** علي الشريط.</span><span class="sxs-lookup"><span data-stu-id="de9c8-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="de9c8-106">حدد خانه الاختيار المجاورة لمجموعه الموقع التي تريد استعادتها.</span><span class="sxs-lookup"><span data-stu-id="de9c8-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="de9c8-107">انقر فوق **استعاده العناصر المحذوفة**.</span><span class="sxs-lookup"><span data-stu-id="de9c8-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="de9c8-108">لاستعاده موقع اتصال محذوف ، يمكنك استخدام مركز مسؤول SharePoint الجديد.</span><span class="sxs-lookup"><span data-stu-id="de9c8-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="de9c8-109">والا ، تحتاج إلى استخدام Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="de9c8-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="de9c8-110">لاستعاده موقع ينتمي إلى مجموعه 365 Office ، تحتاج إلى استعاده المجموعة في مركز مسؤول Exchange.</span><span class="sxs-lookup"><span data-stu-id="de9c8-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="de9c8-111">يمكن استعاده المجموعات لمده 30 يوما بعد ان يتم حذفها.</span><span class="sxs-lookup"><span data-stu-id="de9c8-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

