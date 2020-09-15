---
title: استعاده موقع محذوف
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 570284765f32212b4ef2062db5b70f427b28c121
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47692030"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="7e935-102">استعاده موقع محذوف</span><span class="sxs-lookup"><span data-stu-id="7e935-102">Restore a deleted site</span></span>

<span data-ttu-id="7e935-103">عندما يقوم أحد المسؤولين بحذف موقع SharePoint ، يتم وضعه في سله محذوفات مجموعه المواقع المشتركة ، حيث يتم الاحتفاظ به لمده 93 يوما قبل حذفه بشكل دائم.</span><span class="sxs-lookup"><span data-stu-id="7e935-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="7e935-104">لاستعاده الموقع:</span><span class="sxs-lookup"><span data-stu-id="7e935-104">To restore the site:</span></span>
  
1. <span data-ttu-id="7e935-105">في مركز أداره SharePoint الجديد ، انقر فوق **سله المحذوفات** علي الشريط.</span><span class="sxs-lookup"><span data-stu-id="7e935-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="7e935-106">حدد خانه الاختيار الموجودة إلى جانب مجموعه المواقع المشتركة التي تريد استعادتها.</span><span class="sxs-lookup"><span data-stu-id="7e935-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="7e935-107">انقر فوق **استعاده العناصر المحذوفة**.</span><span class="sxs-lookup"><span data-stu-id="7e935-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="7e935-108">لاستعاده موقع اتصال محذوف ، يمكنك استخدام مركز أداره SharePoint الجديد.</span><span class="sxs-lookup"><span data-stu-id="7e935-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="7e935-109">والا ستحتاج إلى استخدام Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="7e935-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="7e935-110">لاستعاده موقع ينتمي إلى مجموعه Microsoft 365 ، ستحتاج إلى استعاده المجموعة في مركز أداره Exchange.</span><span class="sxs-lookup"><span data-stu-id="7e935-110">To restore a site that belongs to a Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="7e935-111">يمكن استعاده المجموعات لمده 30 يوما بعد حذفها.</span><span class="sxs-lookup"><span data-stu-id="7e935-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

