---
title: 902 (أخطاء المزامنة بسبب الكائنات المكررة)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 6ea833e0c4aebe72bc5c02e3dc10c1edc4136dcc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767102"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="c9865-102">مزامنة الأخطاء بسبب الكائنات المكررة</span><span class="sxs-lookup"><span data-stu-id="c9865-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="c9865-103">قد تتلقى إحدى رسائل الخطأ التالية عند انتهاء مزامنة الدليل في Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="c9865-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="c9865-104">غير قادر على تحديث هذا الكائن في Microsoft Online Services لأن السمات التالية المقترنة بهذا الكائن تحتوي على قيم قد تكون مقترنة بالفعل بكائن آخر في الدليل المحلي.</span><span class="sxs-lookup"><span data-stu-id="c9865-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="c9865-105">يوجد كائن متزامن بنفس عنوان الوكيل بالفعل في دليل خدمات Microsoft عبر الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="c9865-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="c9865-106">غير قادر على تحديث هذا الكائن لأن السمات التالية المقترنة بهذا الكائن لها قيم قد تكون مقترنة بالفعل بكائن آخر في خدمات الدليل المحلي: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="c9865-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="c9865-107">لتحديد المشكلة وإصلاحها، قم بتنزيل وتشغيل [أداة معالجة الأخطاء في IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="c9865-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="c9865-108">لمزيد من المعلومات، راجع [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="c9865-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
