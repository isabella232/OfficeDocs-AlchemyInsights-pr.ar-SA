---
title: إصلاح المشاكل المتعلقة ب علي أجهزة Windows 10 في Microsoft Defender Advanced Threat Protection عن بعد
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
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692431"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a><span data-ttu-id="63782-102">إصلاح المشاكل المتعلقة ب علي أجهزة Windows 10 في Microsoft Defender Advanced Threat Protection عن بعد</span><span class="sxs-lookup"><span data-stu-id="63782-102">Remotely fix problems with onboarding Windows 10 devices to Microsoft Defender Advanced Threat Protection</span></span>

<span data-ttu-id="63782-103">إذا كان بإمكانك الوصول إلى الكمبيوتر البعيد، فاتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="63782-103">If you can access the remote computer, follow these steps:</span></span>

1. <span data-ttu-id="63782-104">قم [بتنزيل أداة](https://go.microsoft.com/fwlink/?linkid=2143466) تشخيص محلل اتصال العميل.</span><span class="sxs-lookup"><span data-stu-id="63782-104">Download the [Client Connectivity Analyzer](https://go.microsoft.com/fwlink/?linkid=2143466) diagnostic tool.</span></span>
2. <span data-ttu-id="63782-105">استخراج MDATPAnalyzer.cmd وتشغيله.</span><span class="sxs-lookup"><span data-stu-id="63782-105">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="63782-106">حدد موقع سجل التشخيص في المجلد MDATPClientAnalyzerResult، وهو المجلد نفسه حيث تم تنزيل أداة "محلل".</span><span class="sxs-lookup"><span data-stu-id="63782-106">Locate the diagnostic log in the MDATPClientAnalyzerResult folder, which is the same folder where the Analyzer tool was downloaded.</span></span>
4. <span data-ttu-id="63782-107">للعثور على مشاكل تتعلق بالاتصال أو إعدادات وكيل الإنترنت، راجع ملف MDATPClientAnalyzer.txt.</span><span class="sxs-lookup"><span data-stu-id="63782-107">To find issues with connectivity or Internet proxy settings, review the log file MDATPClientAnalyzer.txt.</span></span>

<span data-ttu-id="63782-108">لمعرفة المزيد، راجع [المشاكل المتعلقة بآلات التعلية.](https://go.microsoft.com/fwlink/?linkid=2143634)</span><span class="sxs-lookup"><span data-stu-id="63782-108">To learn more, see [Issues with onboarding machines](https://go.microsoft.com/fwlink/?linkid=2143634).</span></span>
