---
title: تكوين الاستثناءات Microsoft Defender ATP المسح الضوئي
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
ms.openlocfilehash: 5eb18f4133aca93c1506f4975c8d0567bede8d57
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543672"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="4d32b-102">تكوين الاستثناءات Microsoft Defender ATP المسح الضوئي</span><span class="sxs-lookup"><span data-stu-id="4d32b-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="4d32b-103">بشكل عام، يمكنك استثناء بعض ملحقات الملفات ومواقع المجلدات من Microsoft Defender ATP المسح الضوئي.</span><span class="sxs-lookup"><span data-stu-id="4d32b-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="4d32b-104">يمكنك أيضا تكوين الاستثناءات للملفات التي يتم فتحها بواسطة عمليات معينة.</span><span class="sxs-lookup"><span data-stu-id="4d32b-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="4d32b-105">لمزيد من المعلومات، [](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) راجع تكوين الاستثناءات والتحقق من صحتها استنادا إلى ملحق الملف وموقع المجلد وتكوين الاستثناءات للملفات التي يتم [فتحها بواسطة العمليات](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span><span class="sxs-lookup"><span data-stu-id="4d32b-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="4d32b-106">لتكوين استثناءات Windows **Server 2016 و2019،** راجع تكوين برنامج الحماية من الفيروسات من Microsoft Defender الاستثناءات على [Windows Server.](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="4d32b-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="4d32b-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="4d32b-107">**Mac**</span></span>

<span data-ttu-id="4d32b-108">للحصول على تفاصيل حول أنواع الاستثناءات المعتمدة وتكوين قائمة [](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) استثناءات ل Mac، راجع أنواع الاستثناءات المعتمدة وكيفية تكوين [قائمة الاستثناءات](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span><span class="sxs-lookup"><span data-stu-id="4d32b-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="4d32b-109">**ملاحظة** يمكنك أيضا التحقق من صحة قوائم الاستثناءات باستخدام ملف اختبار EICAR.</span><span class="sxs-lookup"><span data-stu-id="4d32b-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="4d32b-110">لمزيد من المعلومات، راجع [التحقق من صحة قوائم الاستثناءات باستخدام ملف اختبار EICAR](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="4d32b-110">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="4d32b-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="4d32b-111">**Linux**</span></span>

<span data-ttu-id="4d32b-112">للحصول على تفاصيل حول أنواع الاستثناءات المعتمدة وتكوين قائمة [](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) استثناءات ل Linux، راجع أنواع الاستثناءات المعتمدة وتكوين الاستثناءات والتحقق [من صحتها Microsoft Defender ATP ل Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="4d32b-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="4d32b-113">**ملاحظة** يمكنك أيضا التحقق من صحة قوائم الاستثناءات باستخدام ملف اختبار EICAR.</span><span class="sxs-lookup"><span data-stu-id="4d32b-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="4d32b-114">لمزيد من المعلومات، راجع [التحقق من صحة قوائم الاستثناءات باستخدام ملف اختبار EICAR](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="4d32b-114">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 