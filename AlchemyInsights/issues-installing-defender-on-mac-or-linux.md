---
title: مشاكل في تثبيت Microsoft Defender على Mac أو Linux
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
- "6028"
- "9001222"
ms.openlocfilehash: 39f180852fd0438597fa1ce665b2703fbc7b1aa4
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539667"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a><span data-ttu-id="b0948-102">مشاكل في تثبيت Microsoft Defender على Mac أو Linux</span><span class="sxs-lookup"><span data-stu-id="b0948-102">Issues installing Microsoft Defender on Mac or Linux</span></span>

<span data-ttu-id="b0948-103">**Mac**</span><span class="sxs-lookup"><span data-stu-id="b0948-103">**Mac**</span></span>

- <span data-ttu-id="b0948-104">تأكد من تلبية متطلبات النظام قبل تثبيت Microsoft Defender ATP لنظام التشغيل Mac.</span><span class="sxs-lookup"><span data-stu-id="b0948-104">Ensure that system requirements are met before installing Microsoft Defender ATP for Mac.</span></span> <span data-ttu-id="b0948-105">لمزيد من المعلومات، [راجع كيفية تثبيت Microsoft Defender ATP for Mac](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span><span class="sxs-lookup"><span data-stu-id="b0948-105">For more info, see [How to install Microsoft Defender ATP for Mac](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span></span>  
- <span data-ttu-id="b0948-106">راجع المعلومات في الملف: "/Library/Logs/Microsoft/mdatp/install.log".</span><span class="sxs-lookup"><span data-stu-id="b0948-106">Review the information in the file: "/Library/Logs/Microsoft/mdatp/install.log".</span></span>

<span data-ttu-id="b0948-107">**Linux**</span><span class="sxs-lookup"><span data-stu-id="b0948-107">**Linux**</span></span>

- <span data-ttu-id="b0948-108">تأكد من تلبية متطلبات النظام قبل تثبيت Microsoft Defender ATP ل Linux.</span><span class="sxs-lookup"><span data-stu-id="b0948-108">Ensure that system requirements are met before installing Microsoft Defender ATP for Linux.</span></span> <span data-ttu-id="b0948-109">لمزيد من المعلومات، [راجع كيفية تثبيت MDATP ل Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span><span class="sxs-lookup"><span data-stu-id="b0948-109">For more info, see [How to install MDATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span> 
- <span data-ttu-id="b0948-110">للتحقق من تشغيل خدمة MDATP، راجع [فشل التثبيت](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span><span class="sxs-lookup"><span data-stu-id="b0948-110">To verify that MDATP service is running, see [Installation failed](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span></span>  
    <span data-ttu-id="b0948-111">لا استكشاف الأخطاء وإصلاحها في حالة عدم تشغيل الخدمة، راجع خطوات استكشاف الأخطاء وإصلاحها إذا لم تكن خدمة [mdatp](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)قيد التشغيل.</span><span class="sxs-lookup"><span data-stu-id="b0948-111">To troubleshoot and resolve issues if the service is not running, see [Steps to troubleshoot if mdatp service isn't running](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span></span>
- <span data-ttu-id="b0948-112">للحصول على خطوات للتحقق من تكوين العميل، الذي يتحقق من صحة المنتج، ول تشغيل اختبار الكشف على الملف النصي EICAR، راجع [تكوين العميل](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span><span class="sxs-lookup"><span data-stu-id="b0948-112">For steps to check the client configuration, which verifies the health of the product, and to run a detection test on the EICAR text file, see [Client configuration](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span></span>  

    <span data-ttu-id="b0948-113">**ملاحظة** للحصول على قائمة أنظمة الملفات المعتمدة للنشاط عند الوصول، راجع Microsoft Defender ATP [ل Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span><span class="sxs-lookup"><span data-stu-id="b0948-113">**Note** For a list of supported file systems for on-access activity, see [Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span>