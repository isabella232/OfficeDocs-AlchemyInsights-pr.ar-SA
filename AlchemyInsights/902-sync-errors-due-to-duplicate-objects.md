---
title: 902 (أخطاء المزامنة سبب كائنات مكررة)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: f8db233167a5e2b2ef7290438b8e6d92d0dccb1e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/24/2019
ms.locfileid: "29456371"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="14bbc-102">أخطاء المزامنة نظراً لمضاعفة الكائنات</span><span class="sxs-lookup"><span data-stu-id="14bbc-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="14bbc-103">قد تتلقى إحدى رسائل الخطأ التالية عند انتهاء المزامنة الدليل:</span><span class="sxs-lookup"><span data-stu-id="14bbc-103">You might receive one of the following error messages when directory synchronization finishes:</span></span>
  
- <span data-ttu-id="14bbc-104">غير قادر على تحديث هذا الكائن في خدمة Microsoft لأن القيم التي قد تكون مقترنة بكائن آخر في الدليل المحلي الخاص بك لديه السمات التالية المرتبطة بهذا الكائن.</span><span class="sxs-lookup"><span data-stu-id="14bbc-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>
    
- <span data-ttu-id="14bbc-105">يوجد بالفعل كائن متزامنة بنفس عنوان الوكيل في دليل "خدمات Microsoft عبر إنترنت".</span><span class="sxs-lookup"><span data-stu-id="14bbc-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>
    
- <span data-ttu-id="14bbc-106">غير قادر على تحديث هذا الكائن لأن القيم التي قد تكون مقترنة بكائن آخر في خدمات الدليل المحلي الخاص بك لديه السمات التالية المرتبطة بهذا الكائن: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="14bbc-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>
    
<span data-ttu-id="14bbc-107">لتحديد المشكلة وإصلاحها، تحميل وتشغيل [أداة التحديث خطأ DirSync إيدفيكس](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="14bbc-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>
  
<span data-ttu-id="14bbc-108">لمزيد من المعلومات، انظر [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="14bbc-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
  

