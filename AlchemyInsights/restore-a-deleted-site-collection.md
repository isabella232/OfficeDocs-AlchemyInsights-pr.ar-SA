---
title: استعاده موقع محذوف
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
ms.openlocfilehash: 9e4e9ade058c60ecd7a6ce1b2a40c4996ac5676f
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/18/2019
ms.locfileid: "36552447"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="9b6eb-102">استعاده موقع محذوف</span><span class="sxs-lookup"><span data-stu-id="9b6eb-102">Restore a deleted site</span></span>

<span data-ttu-id="9b6eb-103">عندما يحذف أحد المسؤولين موقعا ، يتم وضعه في سله محذوفات مجموعه الموقع ، حيث يتم الاحتفاظ به لمده 93 يوما قبل حذفه نهائيا.</span><span class="sxs-lookup"><span data-stu-id="9b6eb-103">When an admin deletes a site , it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="9b6eb-104">لاستعاده الموقع:</span><span class="sxs-lookup"><span data-stu-id="9b6eb-104">To restore the site:</span></span>
  
1. <span data-ttu-id="9b6eb-105">في مركز مسؤول SharePoint الجديد ، انقر فوق سله **المحذوفات** علي الشريط.</span><span class="sxs-lookup"><span data-stu-id="9b6eb-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="9b6eb-106">حدد خانه الاختيار المجاورة لمجموعه الموقع التي تريد استعادتها.</span><span class="sxs-lookup"><span data-stu-id="9b6eb-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="9b6eb-107">انقر فوق **استعاده العناصر المحذوفة**.</span><span class="sxs-lookup"><span data-stu-id="9b6eb-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="9b6eb-108">لاستعاده موقع اتصال محذوف ، يمكنك استخدام مركز مسؤول SharePoint الجديد.</span><span class="sxs-lookup"><span data-stu-id="9b6eb-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="9b6eb-109">والا ، تحتاج إلى استخدام Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9b6eb-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="9b6eb-110">لاستعاده موقع ينتمي إلى مجموعه 365 Office ، تحتاج إلى استعاده المجموعة في مركز مسؤول Exchange.</span><span class="sxs-lookup"><span data-stu-id="9b6eb-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="9b6eb-111">يمكن استعاده المجموعات لمده 30 يوما بعد ان يتم حذفها.</span><span class="sxs-lookup"><span data-stu-id="9b6eb-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

