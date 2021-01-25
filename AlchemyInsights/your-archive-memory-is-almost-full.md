---
title: علبه بريد الأرشيف ممتلئة تقريبا
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974149"
---
# <a name="your-archive-mailbox-is-almost-full"></a><span data-ttu-id="db1f9-102">علبه بريد الأرشيف ممتلئة تقريبا</span><span class="sxs-lookup"><span data-stu-id="db1f9-102">Your archive mailbox is almost full</span></span>

<span data-ttu-id="db1f9-103">إذا تلقي المستخدم التحذير ؛ **ان علبه بريد الأرشيف الخاصة بك ممتلئة تقريبا**، أو انك تحتاج إلى زيادة حجم علبه بريد الأرشيف ، اليك بعض التلميحات:</span><span class="sxs-lookup"><span data-stu-id="db1f9-103">If the user receives the warning; **Your archive mailbox is almost full**, or you need to increase the size of their archive mailbox, here are some tips:</span></span>

1. <span data-ttu-id="db1f9-104">إذا تم تعيين Exchange Online للخطة 1 ، فقم بالترقية إلى ترخيص **Exchange online الخطة 2** لزيادة الحجم من 50 غيغابايت إلى 100 غيغابايت.</span><span class="sxs-lookup"><span data-stu-id="db1f9-104">If the user is assigned an Exchange Online Plan 1, upgrade to **Exchange Online Plan 2** license to increase the size from 50 GB to 100GB.</span></span>
1. <span data-ttu-id="db1f9-105">إذا كان المستخدم قد قام بالفعل بتعيين اي من الخيارين التاليين: **Exchange online الخطة 2** أو exchange Online الخطة 1 مع وظيفة اضافيه للارشفه في Exchange online ، استخدم الخطوات التالية لتمكين أرشفه التوسيع التلقائي:.</span><span class="sxs-lookup"><span data-stu-id="db1f9-105">If the user is already assigned either of the following: **Exchange Online Plan 2** or an Exchange Online Plan 1 with an Exchange Online Archiving add-on, use the steps below to enable Auto-Expanding archiving:.</span></span>
 
    1. <span data-ttu-id="db1f9-106">[الاتصال ب Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="db1f9-106">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>
    2. <span data-ttu-id="db1f9-107">قم بتشغيل الكوماندليت التالية للمستخدم:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span><span class="sxs-lookup"><span data-stu-id="db1f9-107">Run the following commandlet for the user:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span></span>
    1. <span data-ttu-id="db1f9-108">قم بتشغيل الكوماندليت التالية لتاكيد تمكينها للمستخدم:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span><span class="sxs-lookup"><span data-stu-id="db1f9-108">Run the following commandlet to confirm it is enabled for the user:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span></span>

<span data-ttu-id="db1f9-109">لمزيد من المعلومات ، راجع:</span><span class="sxs-lookup"><span data-stu-id="db1f9-109">For more information see:</span></span>

- [<span data-ttu-id="db1f9-110"> تمكين الارشفه غير المحدودة-تعليمات المسؤول-توافق Microsoft 365 | مستندات Microsoft</span><span class="sxs-lookup"><span data-stu-id="db1f9-110"> Enable unlimited archiving - Admin Help - Microsoft 365 Compliance | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [<span data-ttu-id="db1f9-111">حدود Exchange Online-أوصاف الخدمة | مستندات Microsoft</span><span class="sxs-lookup"><span data-stu-id="db1f9-111">Exchange Online limits - Service Descriptions | Microsoft Docs</span></span>](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [<span data-ttu-id="db1f9-112">الترقية إلى خطه اعمال مختلفه | مستندات Microsoft</span><span class="sxs-lookup"><span data-stu-id="db1f9-112">Upgrade to a different business plan | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

