---
title: تكوين الاستثناءات لمسح ATP ل Microsoft Defender
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6027"
- "9001464"
ms.openlocfilehash: 912e77b9b1a149fef373f2d0814fb2f0671a48c6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713260"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="a2a12-102">تكوين الاستثناءات لمسح ATP ل Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="a2a12-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="a2a12-103">بشكل عام، يمكنك استبعاد بعض ملحقات الملفات ومواقع المجلدات من عمليات فحص MICROSOFT Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="a2a12-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="a2a12-104">يمكنك أيضا تكوين الاستثناءات للملفات التي يتم فتحها بواسطة عمليات معينة.</span><span class="sxs-lookup"><span data-stu-id="a2a12-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="a2a12-105">لمزيد من المعلومات، [](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) راجع الاستثناءات وتكوينها والتحقق من صحتها استنادا إلى ملحق الملف وموقع المجلد وتكوين الاستثناءات للملفات التي يتم فتحها [بواسطة العمليات.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="a2a12-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="a2a12-106">لتكوين الاستثناءات ل **Windows Server 2016 و2019،** راجع تكوين استثناءات برنامج الحماية من الفيروسات [ل Microsoft Defender على Windows Server.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="a2a12-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="a2a12-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="a2a12-107">**Mac**</span></span>

<span data-ttu-id="a2a12-108">للحصول على تفاصيل حول أنواع الاستثناءات المعتمدة وتكوين قائمة [](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) استثناءات ل Mac، راجع أنواع الاستثناءات المعتمدة وكيفية تكوين قائمة [الاستثناءات.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions)</span><span class="sxs-lookup"><span data-stu-id="a2a12-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="a2a12-109">**ملاحظة** يمكنك أيضا التحقق من صحة قوائم الاستثناءات باستخدام ملف اختبار EICAR.</span><span class="sxs-lookup"><span data-stu-id="a2a12-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="a2a12-110">لمزيد من المعلومات، راجع [التحقق من صحة قوائم الاستثناءات باستخدام ملف اختبار EICAR.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="a2a12-110">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="a2a12-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="a2a12-111">**Linux**</span></span>

<span data-ttu-id="a2a12-112">للحصول على تفاصيل حول أنواع الاستثناءات المعتمدة وتكوين قائمة [](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) استثناءات ل Linux، راجع أنواع الاستثناءات المعتمدة وتكوين استثناءات Microsoft Defender ATP ل Linux والتحقق من [صحتها.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions)</span><span class="sxs-lookup"><span data-stu-id="a2a12-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="a2a12-113">**ملاحظة** يمكنك أيضا التحقق من صحة قوائم الاستثناءات باستخدام ملف اختبار EICAR.</span><span class="sxs-lookup"><span data-stu-id="a2a12-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="a2a12-114">لمزيد من المعلومات، راجع [التحقق من صحة قوائم الاستثناءات باستخدام ملف اختبار EICAR.](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="a2a12-114">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 