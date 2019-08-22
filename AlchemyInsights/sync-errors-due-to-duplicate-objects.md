---
title: 902 (أخطاء المزامنة سبب كائنات مكررة)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 777c2d8d530d03d58180f43b362ee065439b56b3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507402"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="df65f-102">أخطاء المزامنة نظراً لمضاعفة الكائنات</span><span class="sxs-lookup"><span data-stu-id="df65f-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="df65f-103">قد تتلقى إحدى رسائل الخطأ التالية عند انتهاء المزامنة الدليل في Office 365:</span><span class="sxs-lookup"><span data-stu-id="df65f-103">You might receive one of the following error messages when directory synchronization finishes in Office 365:</span></span>

- <span data-ttu-id="df65f-104">غير قادر على تحديث هذا الكائن في خدمة Microsoft لأن القيم التي قد تكون مقترنة بكائن آخر في الدليل المحلي الخاص بك لديه السمات التالية المرتبطة بهذا الكائن.</span><span class="sxs-lookup"><span data-stu-id="df65f-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="df65f-105">يوجد بالفعل كائن متزامنة بنفس عنوان الوكيل في دليل "خدمات Microsoft عبر إنترنت".</span><span class="sxs-lookup"><span data-stu-id="df65f-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="df65f-106">غير قادر على تحديث هذا الكائن لأن القيم التي قد تكون مقترنة بكائن آخر في خدمات الدليل المحلي الخاص بك لديه السمات التالية المرتبطة بهذا الكائن: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="df65f-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="df65f-107">لتحديد المشكلة وإصلاحها، تحميل وتشغيل [أداة التحديث خطأ DirSync إيدفيكس](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="df65f-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="df65f-108">لمزيد من المعلومات، انظر [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="df65f-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
