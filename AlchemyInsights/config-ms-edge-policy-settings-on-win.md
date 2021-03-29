---
title: تكوين إعدادات نهج Microsoft Edge على Windows
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003845"
- "9004632"
- "6894"
- "8358"
ms.openlocfilehash: e9bb489b4d8ecd76fd777ade9fb740ecad542900
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402362"
---
# <a name="configure-microsoft-edge-policy-settings-on-windows"></a><span data-ttu-id="d20c4-102">تكوين إعدادات نهج Microsoft Edge على Windows</span><span class="sxs-lookup"><span data-stu-id="d20c4-102">Configure Microsoft Edge policy settings on Windows</span></span>

<span data-ttu-id="d20c4-103">لتكوين إعدادات النهج والتحديثات المدارة ل Microsoft Edge، استخدم كائنات نهج المجموعة (GPOs).</span><span class="sxs-lookup"><span data-stu-id="d20c4-103">To configure policy settings and managed updates for Microsoft Edge, use Group Policy Objects (GPOs).</span></span> <span data-ttu-id="d20c4-104">يمكنك أيضا توفير النهج من خلال السجل؛ سيكون هذا مناسبا ل (1) أجهزة Windows المنضمة إلى مجال Microsoft Active Directory و(2) مثيلات Windows 10 Pro و Enterprise المسجلين لإدارة الأجهزة في Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="d20c4-104">You can also provision policy through the registry; this would be appropriate for (1) Windows devices joined to a Microsoft Active Directory domain and for (2) Windows 10 Pro and Enterprise instances enrolled for device management in Microsoft Intune.</span></span>

<span data-ttu-id="d20c4-105">لتكوين Microsoft Edge باستخدام GPOs، قم بما يلي:</span><span class="sxs-lookup"><span data-stu-id="d20c4-105">To configure Microsoft Edge by using GPOs, do the following:</span></span>

1. <span data-ttu-id="d20c4-106">انتقل إلى المتجر المركزي لنهية المجموعة في مجال Active Directory، أو إلى مجلد قالب تعريف النهج على أجهزة كمبيوتر فردية، قم بتثبيت كل القوالب الإدارية التي تضيف القواعد والإعدادات ل Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="d20c4-106">Go to the Group Policy Central Store in your Active Directory domain, or to the Policy Definition template folder on individual computers, install all administrative templates that add rules and settings for Microsoft Edge.</span></span>
2. <span data-ttu-id="d20c4-107">قم بتكوين سياسات معينة تريد تعيينها.</span><span class="sxs-lookup"><span data-stu-id="d20c4-107">Configure the specific policies you want to set.</span></span>

<span data-ttu-id="d20c4-108">لمعرفة المزيد، راجع [تكوين إعدادات نهج Microsoft Edge على Windows](https://go.microsoft.com/fwlink/?linkid=2135024).</span><span class="sxs-lookup"><span data-stu-id="d20c4-108">To learn more, see [Configure Microsoft Edge policy settings on Windows](https://go.microsoft.com/fwlink/?linkid=2135024).</span></span>
