---
title: استعادة مجموعة موقع المحذوفة
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 5/1/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: b3c72033dfcc093dd0c2837d2866c6a78d64449c
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/15/2019
ms.locfileid: "28273343"
---
# <a name="restore-a-deleted-site-collection"></a><span data-ttu-id="b66d8-102">استعادة مجموعة موقع المحذوفة</span><span class="sxs-lookup"><span data-stu-id="b66d8-102">Restore a deleted site collection</span></span>

<span data-ttu-id="b66d8-p101">عند حذف مسؤول مجموعة موقع التقليدية، يتم وضعها في مجموعة موقع "سلة المحذوفات"، حيث تظل لأيام 93 قبل إلغائها نهائياً. لاستعادة مجموعة المواقع المشتركة:</span><span class="sxs-lookup"><span data-stu-id="b66d8-p101">When an admin deletes a classic site collection, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted. To restore the site collection:</span></span>
  
1. <span data-ttu-id="b66d8-105">في مركز مسؤول SharePoint الكلاسيكية، انقر فوق **"سلة المحذوفات"** على "الشريط".</span><span class="sxs-lookup"><span data-stu-id="b66d8-105">In the classic SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="b66d8-106">حدد خانة الاختيار المجاورة لمجموعة الموقع التي تريد استعادتها.</span><span class="sxs-lookup"><span data-stu-id="b66d8-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="b66d8-107">انقر فوق **استعادة العناصر المحذوفة**.</span><span class="sxs-lookup"><span data-stu-id="b66d8-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="b66d8-p102">لاستعادة موقع اتصال محذوفة، يمكنك استخدام المعاينة مركز مسؤول SharePoint جديدة. وإلا، تحتاج إلى استخدام PowerShell. لاستعادة موقع الذي ينتمي إلى مجموعة Office 365، تحتاج إلى استعادة المجموعة في مركز مسؤول Exchange. يمكن استعادة مجموعات لمدة 30 يوما بعد أن كنت حذفها.</span><span class="sxs-lookup"><span data-stu-id="b66d8-p102">To restore a deleted communication site, you can use the new SharePoint admin center preview. Otherwise, you need to use PowerShell. To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center. Groups can be restored for 30 days after they're deleted.</span></span>
  

