---
title: مشاكل الأداء ل Microsoft Defender ل Endpoint على Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793544"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="2470a-102">مشاكل الأداء ل Microsoft Defender ل Endpoint على Linux</span><span class="sxs-lookup"><span data-stu-id="2470a-102">Performance issues for Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="2470a-103">ترشدك هذه المقالة عبر خطوات تحديد مشاكل الأداء ل Microsoft Defender ل Endpoint على Linux.</span><span class="sxs-lookup"><span data-stu-id="2470a-103">This article guides you through the steps of identifying performance issues for Microsoft Defender for Endpoint on Linux.</span></span>

<span data-ttu-id="2470a-104">من المهم التحقق أولا من حل المشكلة التي تواجهها باستخدام [الإصدار الأخير.](/microsoft-365/security/defender-endpoint/linux-whatsnew)</span><span class="sxs-lookup"><span data-stu-id="2470a-104">It's important to first verify that the problem you're experiencing is resolved with the [latest version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span></span> 

<span data-ttu-id="2470a-105">لبدء التحقيق، راجع استكشاف مشاكل الأداء وإصلاحها ل [Microsoft Defender ل Endpoint على Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span><span class="sxs-lookup"><span data-stu-id="2470a-105">To start your investigation, see [Troubleshoot performance issues for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span></span>

## <a name="exclusions"></a><span data-ttu-id="2470a-106">الاستثناءات</span><span class="sxs-lookup"><span data-stu-id="2470a-106">Exclusions</span></span>

<span data-ttu-id="2470a-107">يمكن أن تساعد الاستثناءات على الحد من مشاكل الأداء.</span><span class="sxs-lookup"><span data-stu-id="2470a-107">Exclusions can help to mitigate performance issues.</span></span> <span data-ttu-id="2470a-108">راجع استثناءاتك قبل البدء بحيث تكون أي مخاطر إضافية معروفة وموثقة.</span><span class="sxs-lookup"><span data-stu-id="2470a-108">Review your exclusions before you begin so any additional risk is known and documented.</span></span>

<span data-ttu-id="2470a-109">لمزيد من المعلومات، راجع تكوين الاستثناءات ل Microsoft Defender ل Endpoint على Linux والتحقق من [صحتها.](/microsoft-365/security/defender-endpoint/linux-exclusions)</span><span class="sxs-lookup"><span data-stu-id="2470a-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span></span>

<span data-ttu-id="2470a-110">عندما يكون لديك ملفات متعددة & مجلدات يجب استبعادها وكلها على نقطة التركيب نفسها، قد يكون من الأسهل استبعاد نقطة التركيب.</span><span class="sxs-lookup"><span data-stu-id="2470a-110">When you have multiple files & folders to exclude and they're all on the same mountpoint, it might be easier to exclude the mountpoint.</span></span> <span data-ttu-id="2470a-111">بدءا من إصدار فبراير 101.22.80، يمكنك استبعاد نقطة تحميل كاملة.</span><span class="sxs-lookup"><span data-stu-id="2470a-111">Starting with February release 101.22.80, you can exclude an entire mountpoint.</span></span>

<span data-ttu-id="2470a-112">على سبيل المثال، إذا كان /mnt/backup هو نقطة تحميل، يمكنك إضافة /mnt/backup إلى القائمة استبعاد عن طريق تشغيل هذا الأمر:</span><span class="sxs-lookup"><span data-stu-id="2470a-112">For example, if /mnt/backup is a mountpoint, you can add /mnt/backup to the exclude list by running this command:</span></span>

`$ mdatp exclusion folder add –path /mnt/backup`

<span data-ttu-id="2470a-113">**ملاحظة:** تؤدي إضافة استثناءات إلى زيادة خطر عدم الكشف عن البرامج الضارة ويجب معالجتها وتنفيذها بحرص.</span><span class="sxs-lookup"><span data-stu-id="2470a-113">**Note**: Adding exclusions increases the risk of malware not being detected and should be handled and implemented with care.</span></span>

## <a name="need-help"></a><span data-ttu-id="2470a-114">هل تحتاج إلى مساعدة؟</span><span class="sxs-lookup"><span data-stu-id="2470a-114">Need Help?</span></span>

<span data-ttu-id="2470a-115">لمساعدتك بالطريقة الأكثر فعالية، يمكنك تجميع البيانات التشخيصية قبل فتح حالة دعم.</span><span class="sxs-lookup"><span data-stu-id="2470a-115">To assist you in the most efficient way, collect the diagnostic data before opening a support case.</span></span>
