---
title: 902 (أخطاء المزامنة بسبب تكرار الكائنات)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737328"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="45d3a-102">مزامنة الأخطاء بسبب تكرار العناصر</span><span class="sxs-lookup"><span data-stu-id="45d3a-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="45d3a-103">قد تظهر أحدي رسائل الخطا التالية عند انتهاء مزامنة الدليل في Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="45d3a-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="45d3a-104">تعذر تحديث هذا الكائن في خدمات Microsoft عبر الإنترنت لان السمات التالية المقترنة بهذا الكائن تحتوي علي القيم التي قد تكون مقترنة بالفعل بكائن آخر في الدليل المحلي.</span><span class="sxs-lookup"><span data-stu-id="45d3a-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="45d3a-105">يوجد كائن متزامن بنفس عنوان الوكيل بالفعل في دليل Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="45d3a-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="45d3a-106">تعذر تحديث هذا الكائن لان السمات التالية المقترنة بهذا الكائن تحتوي علي القيم التي قد تكون مقترنة بالفعل بكائن آخر في خدمات الدليل المحلي:.</span><span class="sxs-lookup"><span data-stu-id="45d3a-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="45d3a-107">لتحديد المشكلة وإصلاحها ، قم بتنزيل [أداه تحديث الخطا أداه idfix DirSync](https://www.microsoft.com/download/details.aspx?id=36832)وتشغيلها.</span><span class="sxs-lookup"><span data-stu-id="45d3a-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="45d3a-108">لمزيد من المعلومات ، راجع [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="45d3a-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
