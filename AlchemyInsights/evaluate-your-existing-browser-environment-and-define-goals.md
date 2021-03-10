---
title: تقييم بيئة المستعرض الحالية وتحديد الأهداف
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9141"
- "9005291"
ms.openlocfilehash: 5b03d188aa78be83928cf262f1d86f3f933c85ab
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692429"
---
# <a name="evaluate-your-existing-browser-environment-and-define-goals"></a><span data-ttu-id="bdf52-102">تقييم بيئة المستعرض الحالية وتحديد الأهداف</span><span class="sxs-lookup"><span data-stu-id="bdf52-102">Evaluate your existing browser environment and define goals</span></span>

<span data-ttu-id="bdf52-103">يضمن أخذ بعض الوقت لفهم حالة المستعرض الحالية ورؤية المشروع محاذاة جميع المساهمين في المشروع ويعملون نحو نفس الهدف.</span><span class="sxs-lookup"><span data-stu-id="bdf52-103">Taking time to understand your current browser state and project vision ensures all project stakeholders are aligned and are working toward the same goal.</span></span> <span data-ttu-id="bdf52-104">اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="bdf52-104">Follow these steps:</span></span>

1. <span data-ttu-id="bdf52-105">تعريف الحالة الحالية.</span><span class="sxs-lookup"><span data-stu-id="bdf52-105">Define your current state.</span></span> <span data-ttu-id="bdf52-106">فكّر في تنفيذ ما يلي:</span><span class="sxs-lookup"><span data-stu-id="bdf52-106">Consider the following:</span></span>
- <span data-ttu-id="bdf52-107">ما هي المستعرضات التي يتم نشرها حاليا في بيئتك؟</span><span class="sxs-lookup"><span data-stu-id="bdf52-107">Which browsers are currently deployed in your environment?</span></span>
- <span data-ttu-id="bdf52-108">ما المستعرض الذي تم تعيينه كمستعرض افتراضي؟</span><span class="sxs-lookup"><span data-stu-id="bdf52-108">Which browser is set as the default browser?</span></span>
- <span data-ttu-id="bdf52-109">هل تحتاج إلى استخدام Internet Explorer لبعض تطبيقاتك؟</span><span class="sxs-lookup"><span data-stu-id="bdf52-109">Do you need to use Internet Explorer for some of your apps?</span></span>
- <span data-ttu-id="bdf52-110">هل تستخدم قائمة موقع "وضع المؤسسة" لتكوين Internet Explorer اليوم؟</span><span class="sxs-lookup"><span data-stu-id="bdf52-110">Do you use an Enterprise Mode Site List to configure Internet Explorer today?</span></span>
- <span data-ttu-id="bdf52-111">ما هي الأنظمة الأساسية لنظام التشغيل، مثل Windows 10 و macOS، التي تدعمها بيئتك؟</span><span class="sxs-lookup"><span data-stu-id="bdf52-111">Which OS platforms, such as Windows 10 and macOS, does your environment support?</span></span>
- <span data-ttu-id="bdf52-112">ما هي أدوات الإدارة التي تستخدمها لإدارة المستعرض؟</span><span class="sxs-lookup"><span data-stu-id="bdf52-112">Which management tools do you use for browser management?</span></span>
- <span data-ttu-id="bdf52-113">من هو المسؤول عن تكوين المستعرض وإدارته؟</span><span class="sxs-lookup"><span data-stu-id="bdf52-113">Who's responsible for browser configuration and management?</span></span>
- <span data-ttu-id="bdf52-114">ما هي عملية التحقق من توافق المستعرض؟</span><span class="sxs-lookup"><span data-stu-id="bdf52-114">What's the process for validating browser compatibility?</span></span>
2. <span data-ttu-id="bdf52-115">حدد أهداف النشر.</span><span class="sxs-lookup"><span data-stu-id="bdf52-115">Define the goals for your deployment.</span></span> <span data-ttu-id="bdf52-116">ضع الأمور التالية في الاعتبار:</span><span class="sxs-lookup"><span data-stu-id="bdf52-116">Keep the following things in mind:</span></span>
- <span data-ttu-id="bdf52-117">هل تريد تعيين [Microsoft Edge كمستعرض افتراضي؟](https://docs.microsoft.com/DeployEdge/edge-default-browser)</span><span class="sxs-lookup"><span data-stu-id="bdf52-117">Do you want to [set Microsoft Edge as your default browser](https://docs.microsoft.com/DeployEdge/edge-default-browser)?</span></span>
- <span data-ttu-id="bdf52-118">هل تريد إخفاء الإصدار القديم من Microsoft Edge أم تريد تركه [متوفرا للمستخدمين؟](https://docs.microsoft.com/DeployEdge/microsoft-edge-sysupdate-access-old-edge)</span><span class="sxs-lookup"><span data-stu-id="bdf52-118">Do you want to hide the legacy version of Microsoft Edge or do you want to [leave it available for users](https://docs.microsoft.com/DeployEdge/microsoft-edge-sysupdate-access-old-edge)?</span></span>
- <span data-ttu-id="bdf52-119">كيف ستقوم [بتكوين Microsoft Edge؟](https://docs.microsoft.com/DeployEdge/configure-microsoft-edge)</span><span class="sxs-lookup"><span data-stu-id="bdf52-119">How will you [configure Microsoft Edge](https://docs.microsoft.com/DeployEdge/configure-microsoft-edge)?</span></span>
- <span data-ttu-id="bdf52-120">ما هي الميزات الهامة لتكوينها كجزء من النشر الأولي؟</span><span class="sxs-lookup"><span data-stu-id="bdf52-120">What features are critical to configure as part of your initial deployment?</span></span>
- <span data-ttu-id="bdf52-121">ما العملية لمعالجة أي مشاكل تتعلق بالتوافق أو التكوين المحددة؟</span><span class="sxs-lookup"><span data-stu-id="bdf52-121">What is the process for addressing any identified compatibility or configuration issues?</span></span>
3. <span data-ttu-id="bdf52-122">فهم المتطلبات الأساسية للميزات التي قد ترغب في استخدامها، مثل:</span><span class="sxs-lookup"><span data-stu-id="bdf52-122">Understand the prerequisites for features you might want to use, such as:</span></span>
- [<span data-ttu-id="bdf52-123">حماية التطبيقات ل Windows Defender</span><span class="sxs-lookup"><span data-stu-id="bdf52-123">Windows Defender Application Guard</span></span>](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-application-guard/reqs-md-app-guard)
- [<span data-ttu-id="bdf52-124">وضع Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="bdf52-124">Internet Explorer mode</span></span>](https://docs.microsoft.com/DeployEdge/edge-ie-mode)
- [<span data-ttu-id="bdf52-125">المصادقة والمزامنة</span><span class="sxs-lookup"><span data-stu-id="bdf52-125">Authentication and sync</span></span>](https://docs.microsoft.com/DeployEdge/microsoft-edge-security-identity)

<span data-ttu-id="bdf52-126">بعد إكمال هذه الخطوات، تكون جاهزا لبدء التخطيط لاستراتيجية النشر.</span><span class="sxs-lookup"><span data-stu-id="bdf52-126">After you complete these steps, you're ready to start planning your deployment strategy.</span></span>
