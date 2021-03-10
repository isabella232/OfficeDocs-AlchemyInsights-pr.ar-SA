---
title: إيقاف تشغيل الأجهزة غير التي تعمل بنظام التشغيل Windows من Microsoft Defender Advanced Threat Protection (ATP)
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
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692456"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="9574f-102">إيقاف تشغيل الأجهزة غير التي تعمل بنظام التشغيل Windows من Microsoft Defender Advanced Threat Protection (ATP)</span><span class="sxs-lookup"><span data-stu-id="9574f-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="9574f-103">إليك كيفية تنفيذ ذلك:</span><span class="sxs-lookup"><span data-stu-id="9574f-103">Here's how:</span></span>

1. <span data-ttu-id="9574f-104">اتبع وثائق جهة خارجية لقطع اتصال حل جهة خارجية من Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="9574f-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="9574f-105">من مستأجر Azure Active Directory، قم بإزالة الأذونات الخاصة بالحل الخاص ب جهة خارجية:</span><span class="sxs-lookup"><span data-stu-id="9574f-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="9574f-106">سجل الدخول إلى [مدخل Azure.](https://go.microsoft.com/fwlink/?linkid=2125612)</span><span class="sxs-lookup"><span data-stu-id="9574f-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="9574f-107">حدد **كل الخدمات**  >  **Azure Active Directory**  >  **Enterprise Applications.**</span><span class="sxs-lookup"><span data-stu-id="9574f-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="9574f-108">حدد التطبيق الذي تريد إيقاف تشغيله.</span><span class="sxs-lookup"><span data-stu-id="9574f-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="9574f-109">حدد **"حذف".**</span><span class="sxs-lookup"><span data-stu-id="9574f-109">Select **Delete**.</span></span>

<span data-ttu-id="9574f-110">لمعرفة المزيد، راجع [Offboard غير أجهزة Windows.](https://go.microsoft.com/fwlink/?linkid=2143630)</span><span class="sxs-lookup"><span data-stu-id="9574f-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
