---
title: تكوين استثناءات MDATP والتحقق من صحتها على جهاز Linux
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
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/09/2021
ms.locfileid: "50692626"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a><span data-ttu-id="bf327-102">تكوين استثناءات MDATP والتحقق من صحتها على جهاز Linux</span><span class="sxs-lookup"><span data-stu-id="bf327-102">Configure and validate exclusions for MDATP on a Linux machine</span></span>

<span data-ttu-id="bf327-103">يمكنك استبعاد بعض الملفات والمجلدات والعمليات والملفات التي تم فتحها من خلال عمليات فحص MDATP.</span><span class="sxs-lookup"><span data-stu-id="bf327-103">You can exclude certain files, folders, processes, and process-opened files from MDATP scans.</span></span> <span data-ttu-id="bf327-104">تساعد الاستثناءات في منع الكشف غير الصحيح عن البرامج والملفات الفريدة أو المخصصة لم مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="bf327-104">Exclusions help prevent incorrect detection of software and files unique or customized to your organization.</span></span> <span data-ttu-id="bf327-105">تساعد الاستثناءات أيضا على الحد من مشاكل الأداء التي تسببها MDATP.</span><span class="sxs-lookup"><span data-stu-id="bf327-105">Exclusions also help mitigate performance problems caused by MDATP.</span></span>

<span data-ttu-id="bf327-106">لمعرفة المزيد، راجع [تكوين استثناءات MDATP ل Linux](https://go.microsoft.com/fwlink/?linkid=2144517)والتحقق من صحتها.</span><span class="sxs-lookup"><span data-stu-id="bf327-106">To learn more, see [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="bf327-107">لا تنطبق الاستثناءات الموضحة في هذه المقالة على إمكانيات MDATP الأخرى ل Linux، بما في ذلك الكشف عن نقطة النهاية والاستجابة (EDR).</span><span class="sxs-lookup"><span data-stu-id="bf327-107">The exclusions described in this article don't apply to other capabilities of MDATP for Linux, including endpoint detection and response (EDR).</span></span> <span data-ttu-id="bf327-108">يمكن أن تقوم الملفات التي تستبعدها باستخدام الأساليب الموضحة في هذه المقالة بتشغيل تنبيهات EDR وإمكانيات الكشف الأخرى.</span><span class="sxs-lookup"><span data-stu-id="bf327-108">Files that you exclude by using the methods described in this article can still trigger EDR alerts and other detection capabilities.</span></span>
