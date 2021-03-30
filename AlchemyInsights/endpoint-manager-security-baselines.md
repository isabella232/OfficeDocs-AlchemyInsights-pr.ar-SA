---
title: EndPoint Manager - خطوط الأمان الأساسية
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/29/2021
ms.locfileid: "51420691"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="07af4-102">EndPoint Manager - خطوط الأمان الأساسية</span><span class="sxs-lookup"><span data-stu-id="07af4-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="07af4-103">إن خطوط الأمان الأساسية هي مجموعات مكونة مسبقا من إعدادات Windows تساعدك على تطبيق إعدادات الأمان الموصى بها من قبل فرق الأمان ذات الصلة.</span><span class="sxs-lookup"><span data-stu-id="07af4-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="07af4-104">يمكن تخصيص هذه الأساسات لتقديم الإعدادات والقيم المطلوبة فقط.</span><span class="sxs-lookup"><span data-stu-id="07af4-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="07af4-105">لمزيد من المعلومات حول خطوط الأمان الأساسية، راجع استخدام خطوط الأمان الأساسية لتكوين أجهزة [Windows 10 في Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="07af4-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="07af4-106">توجد حاليا خطوط أساسية لهذه المنتجات:</span><span class="sxs-lookup"><span data-stu-id="07af4-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="07af4-107">إعدادات أمان Windows MDM</span><span class="sxs-lookup"><span data-stu-id="07af4-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="07af4-108">Microsoft Defender for EndPoint Security</span><span class="sxs-lookup"><span data-stu-id="07af4-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="07af4-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="07af4-109">Microsoft Edge</span></span>

<span data-ttu-id="07af4-110">يتم تحديث كل أساس بشكل دوري، كما يتم إصداره في إصدارات تزايدية.</span><span class="sxs-lookup"><span data-stu-id="07af4-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="07af4-111">يضيف كل إصدار الإعدادات أو يزيلها من الإصدار السابق للتأكد من أن الأساس يلبي الإرشادات الحالية.</span><span class="sxs-lookup"><span data-stu-id="07af4-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="07af4-112">تسمح وحدة تحكم خطوط الأمان الأساسية في أمان نقطة النهاية بمقارنة إصدارات مختلفة عن طريق جعل التغييرات من إصدار إلى إصدار مرئية.</span><span class="sxs-lookup"><span data-stu-id="07af4-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="07af4-113">للحصول على إرشادات حول كيفية تغيير إصدار الأساس الذي يتم نشره بفعالية أكبر، راجع إدارة ملفات تعريف خط الأمان الأساسي [في Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="07af4-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="07af4-114">بعد نشر أساس أمان، يمكنك مراقبة حالة النشر ومراجعة الإعدادات على أساس كل جهاز على حدة.</span><span class="sxs-lookup"><span data-stu-id="07af4-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="07af4-115">**ملاحظة:** قد تستغرق بيانات إعداد التقارير لخط الأساسات ما يصل إلى 24 ساعة لكي تظهر من النشر الأولي إلى جهاز، وما يصل إلى 6 ساعات لمزيد من التحديثات.</span><span class="sxs-lookup"><span data-stu-id="07af4-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="07af4-116">السبب الأكثر شيوعا لعدم تطبيق إعداد الأساس هو أن نفس الإعداد يتم استخدامه في ملف تعريف مختلف.</span><span class="sxs-lookup"><span data-stu-id="07af4-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="07af4-117">يمكن التحقق من هذا السيناريو لجهاز معين عن طريق تحديد هذا الجهاز من ضمن عقدة حالة الجهاز لملف تعريف أساسي الأمان.</span><span class="sxs-lookup"><span data-stu-id="07af4-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="07af4-118">للحصول على التفاصيل، راجع [حل التعارضات الخاصة باساسيات الأمان](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span><span class="sxs-lookup"><span data-stu-id="07af4-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>