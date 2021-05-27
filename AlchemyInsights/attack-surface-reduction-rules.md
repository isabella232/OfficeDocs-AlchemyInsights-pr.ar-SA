---
title: قواعد الحد من سطح الهجوم
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676043"
---
# <a name="attack-surface-reduction-rules"></a><span data-ttu-id="00682-102">قواعد الحد من سطح الهجوم</span><span class="sxs-lookup"><span data-stu-id="00682-102">Attack surface reduction rules</span></span>

<span data-ttu-id="00682-103">يمكن أن يقلل استبعاد الملفات أو المجلدات بشدة من الحماية التي توفرها قواعد تقليل مساحة الهجوم.</span><span class="sxs-lookup"><span data-stu-id="00682-103">Excluding files or folders can severely reduce the protection provided by attack surface reduction rules.</span></span> <span data-ttu-id="00682-104">يسمح بتشغيل الملفات التي تم حظرها بواسطة قاعدة، ولا يتم تسجيل أي تقرير أو حدث.</span><span class="sxs-lookup"><span data-stu-id="00682-104">Files that would have been blocked by a rule are allowed to run, and no report or event is recorded.</span></span> <span data-ttu-id="00682-105">ينطبق الاستثناء على كل القواعد التي تسمح بالاستثناءات.</span><span class="sxs-lookup"><span data-stu-id="00682-105">An exclusion applies to all rules that allow exclusions.</span></span>

<span data-ttu-id="00682-106">تستخدم استثناءات ASR بناء الجملة نفسه الذي تستخدمه برنامج الحماية من الفيروسات من Microsoft Defender استثناءات.</span><span class="sxs-lookup"><span data-stu-id="00682-106">ASR exclusions use the same syntax as Microsoft Defender Antivirus exclusions.</span></span> <span data-ttu-id="00682-107">للحصول على التفاصيل، راجع [تكوين الاستثناءات](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus)لمسح برنامج الحماية من الفيروسات من Microsoft Defender والتحقق من صحتها .</span><span class="sxs-lookup"><span data-stu-id="00682-107">For details, see [Configure and validate exclusions for Microsoft Defender Antivirus scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span></span> <span data-ttu-id="00682-108">لتجنب المشاكل، راجع [الأخطاء الشائعة لتجنبها عند تعريف الاستثناءات.](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="00682-108">To avoid problems, review [Common mistakes to avoid when defining exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="00682-109">لا تدعم كل قواعد ASR الاستثناءات.</span><span class="sxs-lookup"><span data-stu-id="00682-109">Not all ASR rules support exclusions.</span></span> <span data-ttu-id="00682-110">للتحقق من صحة ما إذا كانت القاعدة تدعم الاستثناءات، راجع الجدول قواعد تقليل مساحة [الهجوم](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span><span class="sxs-lookup"><span data-stu-id="00682-110">To validate if your rule supports exclusions, see the table [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

## <a name="attack-surface-reduction-rules"></a><span data-ttu-id="00682-111">قواعد الحد من سطح الهجوم</span><span class="sxs-lookup"><span data-stu-id="00682-111">Attack surface reduction rules</span></span>

<span data-ttu-id="00682-112">يتضمن سطح هجوم مؤسستك كل الأماكن التي يمكن أن يعرض فيها مهاجم أجهزة المؤسسة أو شبكاتها للخطر.</span><span class="sxs-lookup"><span data-stu-id="00682-112">Your organization attack surface includes all the places where an attacker could compromise organization devices or networks.</span></span> <span data-ttu-id="00682-113">يعني تقليل سطح الهجوم حماية أجهزة المؤسسة وشبكة الاتصال، مما يترك للمهاجمين طرقا أقل لتنفيذ الهجمات.</span><span class="sxs-lookup"><span data-stu-id="00682-113">Reducing your attack surface means protecting the organization devices and network, which leaves attackers with fewer ways to perform attacks.</span></span> <span data-ttu-id="00682-114">يمكن أن يساعدك تكوين قواعد تقليل مساحة الهجوم في Microsoft Defender ل Endpoint.</span><span class="sxs-lookup"><span data-stu-id="00682-114">Configuring attack surface reduction rules in Microsoft Defender for Endpoint can help.</span></span>

<span data-ttu-id="00682-115">لمزيد من المعلومات، اطلع على:</span><span class="sxs-lookup"><span data-stu-id="00682-115">For more information, see:</span></span>

- [<span data-ttu-id="00682-116">تعيين قاعدة ASR GUID إلى الاسم</span><span class="sxs-lookup"><span data-stu-id="00682-116">Map ASR rule GUID to name</span></span>](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- <span data-ttu-id="00682-117">متطلبات قواعد ASR:</span><span class="sxs-lookup"><span data-stu-id="00682-117">ASR rules requirements:</span></span>
    - [<span data-ttu-id="00682-118">Windows 10 Pro الإصدار 1709 أو الإصدارات الأحدث</span><span class="sxs-lookup"><span data-stu-id="00682-118">Windows 10 Pro, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="00682-119">Windows 10 Enterprise الإصدار 1709 أو الإصدارات الأحدث</span><span class="sxs-lookup"><span data-stu-id="00682-119">Windows 10 Enterprise, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="00682-120">Windows الخادم، الإصدار 1803 (قناة نصف سنوية) أو إصدار أحدث</span><span class="sxs-lookup"><span data-stu-id="00682-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span></span>](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a><span data-ttu-id="00682-121">تحديد الاستثناء الصحيح الذي يجب تطبيقه</span><span class="sxs-lookup"><span data-stu-id="00682-121">Identify the correct exclusion to apply</span></span>

1. <span data-ttu-id="00682-122">ابحث عن eventID 1121 أو 1122 في سجل Microsoft-Windows-Windows Defender/Operational.</span><span class="sxs-lookup"><span data-stu-id="00682-122">Look for eventID 1121 or 1122 in the Microsoft-Windows-Windows Defender/Operational log.</span></span>

1. <span data-ttu-id="00682-123">قم بتقييم سيناريو الكتلة وسياقها وتأكد من أنه يجب إلغاء حظر هذا السيناريو.</span><span class="sxs-lookup"><span data-stu-id="00682-123">Evaluate the block scenario and context and confirm that this scenario needs to be unblocked.</span></span>

1. <span data-ttu-id="00682-124">اقرأ القيمة Path في تفاصيل الحدث، وهي القيمة التي تعرف الاستثناء.</span><span class="sxs-lookup"><span data-stu-id="00682-124">Read the Path value in the event details, which is the value that defines the exclusion.</span></span>
    - <span data-ttu-id="00682-125">اجعل الاستثناء صارما قدر الإمكان.</span><span class="sxs-lookup"><span data-stu-id="00682-125">Make the exclusion as strict as possible.</span></span>
    - <span data-ttu-id="00682-126">تطبيق أحرف بدل عند الحاجة (على سبيل المثال، استبدال متغير المستخدم).</span><span class="sxs-lookup"><span data-stu-id="00682-126">Apply a wildcard where needed (for example, replace User variable).</span></span>

1. <span data-ttu-id="00682-127">طبق الاستثناء وفقا لاحتياجات النشر.</span><span class="sxs-lookup"><span data-stu-id="00682-127">Apply the exclusion according to your deployment needs.</span></span> <span data-ttu-id="00682-128">للحصول على التفاصيل، راجع [تخصيص قواعد تقليل مساحة الهجوم](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span><span class="sxs-lookup"><span data-stu-id="00682-128">For details, see [Customize attack surface reduction rules](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span></span>

## <a name="exclusion-is-not-honored"></a><span data-ttu-id="00682-129">لا يتم احترام الاستثناء</span><span class="sxs-lookup"><span data-stu-id="00682-129">Exclusion is not honored</span></span>

1. <span data-ttu-id="00682-130">تحديد ما إذا كانت القاعدة تدعم الاستثناءات أم لا.</span><span class="sxs-lookup"><span data-stu-id="00682-130">Determine whether the rule support exclusions.</span></span> <span data-ttu-id="00682-131">للحصول على التفاصيل، راجع [قواعد تقليل مساحة الهجوم](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span><span class="sxs-lookup"><span data-stu-id="00682-131">For details, see [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

1. <span data-ttu-id="00682-132">راجع الاستثناءات المطبقة وتحقق من بيانات الحدث بسبب الأخطاء المطبعية أو أحرف البدل التي تم تفسيرها بشكل خاطئ.</span><span class="sxs-lookup"><span data-stu-id="00682-132">Review the exclusions applied and verify with the event data for typos or misinterpreted wildcards.</span></span> <span data-ttu-id="00682-133">لمزيد من المعلومات، راجع [أنواع الاستثناءات المعتمدة](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="00682-133">For more info, see [Supported exclusion types](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span></span>

1. <span data-ttu-id="00682-134">إذا كان تأثير القاعدة عال جدا، فراجع نقل القاعدة (للخلف) إلى وضع التدقيق لتنفيذ المزيد من التحقق من الصحة.</span><span class="sxs-lookup"><span data-stu-id="00682-134">if the impact of the rule it too high, consider moving the rule (back) to Audit mode to perform further validation.</span></span> <span data-ttu-id="00682-135">للحصول على التفاصيل، راجع [اختبار كيفية عمل ميزات Microsoft Defender لنقطة النهاية في وضع التدقيق](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span><span class="sxs-lookup"><span data-stu-id="00682-135">For details, see [Test how Microsoft Defender for Endpoint features work in audit mode](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span></span>

1. <span data-ttu-id="00682-136">تجميع بيانات الدعم لفتح حالة دعم باستخدام هذا الأمر:</span><span class="sxs-lookup"><span data-stu-id="00682-136">Collect support data to open a support case by using this command:</span></span>
    
   <span data-ttu-id="00682-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span><span class="sxs-lookup"><span data-stu-id="00682-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span></span>

    <span data-ttu-id="00682-138">لمزيد من المعلومات، راجع المشاكل المتعلقة [بآلات التكوين في Microsoft Defender لنقاط النهاية](issues-with-onboarding-machines.md).</span><span class="sxs-lookup"><span data-stu-id="00682-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span></span>
