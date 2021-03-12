---
title: إصلاح قواعد النقل
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743393"
---
# <a name="fix-transport-rules"></a><span data-ttu-id="b4503-102">إصلاح قواعد النقل</span><span class="sxs-lookup"><span data-stu-id="b4503-102">Fix transport rules</span></span>

<span data-ttu-id="b4503-103">أثرت قاعدة تدفق بريد مخصصة على هذه الرسالة.</span><span class="sxs-lookup"><span data-stu-id="b4503-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="b4503-104">لمراجعة القاعدة بدقة، يمكنك القيام بما يلي:</span><span class="sxs-lookup"><span data-stu-id="b4503-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="b4503-105">في نتائج الإرسال، ضمن **معلومات إضافية،** لاحظ **GUID** أو **اسم النهج**.</span><span class="sxs-lookup"><span data-stu-id="b4503-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="b4503-106">تشغيل Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="b4503-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="b4503-107">لمزيد من المعلومات، [راجع فتح Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="b4503-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="b4503-108">تشغيل هذا الأمر (باستخدام GUID من الإرسال): **Get-TransportRule -identity "GUID"** | fl \* الوصف\*</span><span class="sxs-lookup"><span data-stu-id="b4503-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="b4503-109">راجع الوصف لرؤية الشروط التي تم تكوينها التي أثرت على الرسالة.</span><span class="sxs-lookup"><span data-stu-id="b4503-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="b4503-110">لمعرفة المزيد، راجع [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span><span class="sxs-lookup"><span data-stu-id="b4503-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>
