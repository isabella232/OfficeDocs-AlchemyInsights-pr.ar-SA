---
title: تكوين إعدادات نهج Microsoft Edge علي Windows
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
- "6894"
ms.openlocfilehash: 7f626152c3833638436dfe05e8dcd13fc86ef594
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583156"
---
# <a name="configure-microsoft-edge-policy-settings-on-windows"></a><span data-ttu-id="f899c-102">تكوين إعدادات نهج Microsoft Edge علي Windows</span><span class="sxs-lookup"><span data-stu-id="f899c-102">Configure Microsoft Edge policy settings on Windows</span></span>

<span data-ttu-id="f899c-103">لتكوين إعدادات النهج والتحديثات المدارة ل Microsoft Edge ، استخدم كائنات نهج المجموعة (GPOs).</span><span class="sxs-lookup"><span data-stu-id="f899c-103">To configure policy settings and managed updates for Microsoft Edge, use Group Policy Objects (GPOs).</span></span> <span data-ttu-id="f899c-104">يمكنك أيضا توفير النهج من خلال السجل ؛ سيكون هذا مناسبا ل (1) الاجهزه التي تعمل بنظام التشغيل Windows والمتصلة بمجال Microsoft Active directory النسبة ل (2) التي تم تسجيلها لأداره الاجهزه في Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="f899c-104">You can also provision policy through the registry; this would be appropriate for (1) Windows devices joined to a Microsoft Active Directory domain and for (2) Windows 10 Pro and Enterprise instances enrolled for device management in Microsoft Intune.</span></span>

<span data-ttu-id="f899c-105">لتكوين Microsoft Edge باستخدام GPOs ، قم بما يلي:</span><span class="sxs-lookup"><span data-stu-id="f899c-105">To configure Microsoft Edge by using GPOs, do the following:</span></span>

1. <span data-ttu-id="f899c-106">للحصول علي المخزن المركزي لنهج المجموعة في مجال Active Directory ، أو إلى مجلد قالب تعريف النهج علي أجهزه الكمبيوتر الفردية ، قم بتثبيت كل القوالب الاداريه التي تضيف قواعد وإعدادات ل Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="f899c-106">To the Group Policy Central Store in your Active Directory domain, or to the Policy Definition template folder on individual computers, install all administrative templates that add rules and settings for Microsoft Edge.</span></span>
2. <span data-ttu-id="f899c-107">قم بتكوين النهج المعينة التي تريد تعيينها.</span><span class="sxs-lookup"><span data-stu-id="f899c-107">Configure the specific policies you want to set.</span></span>

<span data-ttu-id="f899c-108">لمعرفه المزيد ، راجع [تكوين إعدادات نهج Microsoft Edge علي Windows](https://go.microsoft.com/fwlink/?linkid=2135024).</span><span class="sxs-lookup"><span data-stu-id="f899c-108">To learn more, see [Configure Microsoft Edge policy settings on Windows](https://go.microsoft.com/fwlink/?linkid=2135024).</span></span>
