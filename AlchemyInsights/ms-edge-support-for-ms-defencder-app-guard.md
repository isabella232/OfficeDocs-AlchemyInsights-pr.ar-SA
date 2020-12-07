---
title: دعم microsoft Edge لحماية التطبيقات ل Microsoft Defender
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
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583177"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a><span data-ttu-id="dd485-102">دعم microsoft Edge لحماية التطبيقات ل Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="dd485-102">Microsoft Edge's support for Microsoft Defender Application Guard</span></span>

<span data-ttu-id="dd485-103">مصمم لنظام التشغيل Windows 10 و Microsoft Edge ، يستخدم "حماية التطبيقات" أسلوب عزل الاجهزه الذي يسمح للمستخدم بالتنقل في موقع غير موثوق به من داخل حاويه معزولة ومتوافقة مع Hyper-v ، مفصوله عن نظام التشغيل المضيف.</span><span class="sxs-lookup"><span data-stu-id="dd485-103">Designed for Windows 10 and Microsoft Edge, Application Guard uses a hardware-isolation approach that lets a user navigate an untrusted site from inside an isolated, Hyper-V–enabled container, separated from the host operating system.</span></span>

<span data-ttu-id="dd485-104">يحدد مسؤول المؤسسة قائمه بمواقع ويب الموثوق بها وموارد السحابة والشبكات الداخلية.</span><span class="sxs-lookup"><span data-stu-id="dd485-104">An enterprise admin defines a list of trusted websites, cloud resources, and internal networks.</span></span> <span data-ttu-id="dd485-105">عندما يقوم أحد المستخدمين بزيارة موقع غير موجود في القائمة ، سيفتح Microsoft Edge الموقع في الحاوية.</span><span class="sxs-lookup"><span data-stu-id="dd485-105">When a user visits a site that's not on the list, Microsoft Edge will open the site in the container.</span></span> <span data-ttu-id="dd485-106">وهذا يعني انه في حاله توقف الموقع عن العمل ، سيظل الكمبيوتر المضيف محميا ولن يتمكن المهاجم من الوصول إلى بيانات المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="dd485-106">This means that if the site turns out to be malicious, the host PC will remain protected and the attacker won't get to the enterprise data.</span></span>

<span data-ttu-id="dd485-107">يتم اعتماد تثبيت الملحقات في الحاوية من Microsoft Edge الإصدار 81 ، ويمكن التحكم فيه عبر النهج.</span><span class="sxs-lookup"><span data-stu-id="dd485-107">Installation of extensions in the container is supported as of Microsoft Edge version 81, and it can be controlled via a policy.</span></span> <span data-ttu-id="dd485-108">يجب ان تتم أضافه عنوان أوبداتيورل الذي يتم استخدامه في نهج اكستينسيونينستالفورسيليست كمورد حيادي في نهج عزل الشبكة المستخدمة من قبل حماية التطبيقات.</span><span class="sxs-lookup"><span data-stu-id="dd485-108">The updateURL address that gets used in the ExtensionInstallForcelist policy should be added as a Neutral Resource in the Network Isolation policies used by Application Guard.</span></span>

<span data-ttu-id="dd485-109">للحصول علي مزيد من المعلومات ، راجع [دعم Microsoft Edge لحماية التطبيقات ل Microsoft Defender](https://go.microsoft.com/fwlink/?linkid=2134229).</span><span class="sxs-lookup"><span data-stu-id="dd485-109">For more info, see [Microsoft Edge support for Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span></span>
