---
title: إدارة نقاط النهاية - أساسات الأمان
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
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440854"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="8b74e-102">إدارة نقاط النهاية - أساسات الأمان</span><span class="sxs-lookup"><span data-stu-id="8b74e-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="8b74e-103">أساسات الأمان هي مجموعات من إعدادات Windows مكوّنة مسبقاً تساعدك على تطبيق إعدادات الأمان التي يوصي بها فرق الأمان ذات الصلة.</span><span class="sxs-lookup"><span data-stu-id="8b74e-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="8b74e-104">يمكن تخصيص هذه الأساسات لتقديم الإعدادات والقيم المرادة فقط.</span><span class="sxs-lookup"><span data-stu-id="8b74e-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="8b74e-105">للحصول على مزيد من المعلومات حول أساسات الأمان، اطلع على [استخدام أساسات الأمان لتكوين أجهزة Windows 10 في Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="8b74e-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="8b74e-106">متوفر حالياً أساسات لهذه البرامج:</span><span class="sxs-lookup"><span data-stu-id="8b74e-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="8b74e-107">إعدادات أمان Windows MDM</span><span class="sxs-lookup"><span data-stu-id="8b74e-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="8b74e-108">أمان Microsoft Defender لنقطة النهاية</span><span class="sxs-lookup"><span data-stu-id="8b74e-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="8b74e-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="8b74e-109">Microsoft Edge</span></span>

<span data-ttu-id="8b74e-110">يُحدث كل أساس بشكل دوري ويطرح في الإصدارات المتزايدة.</span><span class="sxs-lookup"><span data-stu-id="8b74e-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="8b74e-111">يضيف كل إصدار إعدادات من الإصدار السابق أو يزيلها لضمان استيفاء الأساس الإرشادات الحالية.</span><span class="sxs-lookup"><span data-stu-id="8b74e-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="8b74e-112">تسمح وحدة التحكم في أساسات الأمان في أمان نقطة النهاية بالمقارنة بين الإصدارات المختلفة بإظهار التغييرات من إصدار إلى آخر.</span><span class="sxs-lookup"><span data-stu-id="8b74e-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="8b74e-113">للحصول على إرشادات حول كيفية تغيير إصدار الأساس الذي سيتم نشره بأعلى فاعلية، اطلع على [إدارة ملفات تعريف أساسات الأمان في Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="8b74e-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="8b74e-114">بعد نشر أحد أساسات الأمان، ستتمكّن من مراقبة حالة النشر ومراجعة الإعدادات على الأجهزة بشكل مستقل.</span><span class="sxs-lookup"><span data-stu-id="8b74e-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="8b74e-115">**ملاحظة:** قد يستغرق ظهور بيانات تقارير الأساسات من النشر الأولي إلى أحد الأجهزة ما يصل إلى 24 ساعة وقد يستغرق إجراء تحديثات إضافية ما يصل إلى 6 ساعات.</span><span class="sxs-lookup"><span data-stu-id="8b74e-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="8b74e-116">يكّمن السبب الأكثر شيوعاً وراء عدم تطبيق أحد إعدادات الأساسات في أن الإعداد نفسه يُستخدم حالياً في ملف تعريف مختلف.</span><span class="sxs-lookup"><span data-stu-id="8b74e-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="8b74e-117">يمكن التحقق من هذا السيناريو لجهاز معين من خلال تحديد هذا الجهاز من داخل عقدة "حالة الجهاز" لملف تعريف أساس الأمان.</span><span class="sxs-lookup"><span data-stu-id="8b74e-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="8b74e-118">للحصول على التفاصيل، اطلع على [حل التعارضات بين أساسات الأمان](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span><span class="sxs-lookup"><span data-stu-id="8b74e-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>