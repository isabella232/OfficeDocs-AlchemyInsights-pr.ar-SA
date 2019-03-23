---
title: 902 (أخطاء المزامنة سبب كائنات مكررة)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: eac74a6d4de58c9cdbdc8e8df8f705293bb12e87
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/22/2019
ms.locfileid: "30781249"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="843bd-102">أخطاء المزامنة نظراً لمضاعفة الكائنات</span><span class="sxs-lookup"><span data-stu-id="843bd-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="843bd-103">قد تتلقى إحدى رسائل الخطأ التالية عند انتهاء المزامنة الدليل:</span><span class="sxs-lookup"><span data-stu-id="843bd-103">You might receive one of the following error messages when directory synchronization finishes:</span></span>
  
- <span data-ttu-id="843bd-104">غير قادر على تحديث هذا الكائن في خدمة Microsoft لأن القيم التي قد تكون مقترنة بكائن آخر في الدليل المحلي الخاص بك لديه السمات التالية المرتبطة بهذا الكائن.</span><span class="sxs-lookup"><span data-stu-id="843bd-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>
    
- <span data-ttu-id="843bd-105">يوجد بالفعل كائن متزامنة بنفس عنوان الوكيل في دليل "خدمات Microsoft عبر إنترنت".</span><span class="sxs-lookup"><span data-stu-id="843bd-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>
    
- <span data-ttu-id="843bd-106">غير قادر على تحديث هذا الكائن لأن القيم التي قد تكون مقترنة بكائن آخر في خدمات الدليل المحلي الخاص بك لديه السمات التالية المرتبطة بهذا الكائن: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="843bd-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>
    
<span data-ttu-id="843bd-107">لتحديد المشكلة وإصلاحها، تحميل وتشغيل [أداة التحديث خطأ DirSync إيدفيكس](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="843bd-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>
  
<span data-ttu-id="843bd-108">لمزيد من المعلومات، انظر [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="843bd-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
  

