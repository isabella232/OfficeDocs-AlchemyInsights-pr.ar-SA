---
title: لا تعمل المؤشرات باستخدام مستعرض Edge
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
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676045"
---
# <a name="indicators-dont-work-using-edge-browser"></a><span data-ttu-id="1be02-102">لا تعمل المؤشرات باستخدام مستعرض Edge</span><span class="sxs-lookup"><span data-stu-id="1be02-102">Indicators don't work using Edge browser</span></span>

<span data-ttu-id="1be02-103">بعد إنشاء مؤشر، لن يتم احترامه بواسطة Edge (الشاشة الذكية).</span><span class="sxs-lookup"><span data-stu-id="1be02-103">After you created an Indicator, it's not honored by Edge (Smartscreen).</span></span> <span data-ttu-id="1be02-104">لمزيد من المعلومات، راجع [إنشاء مؤشرات ل IPs وURLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span><span class="sxs-lookup"><span data-stu-id="1be02-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>

## <a name="step-1-ensure-the-following"></a><span data-ttu-id="1be02-105">الخطوة 1: التأكد من ما يلي</span><span class="sxs-lookup"><span data-stu-id="1be02-105">Step 1: Ensure the following</span></span>

- <span data-ttu-id="1be02-106">تحقق من صحة المؤشر (لا توجد أخطاء كتابية في IP/URL، الإجراء الصحيح، مجموعات RBAC الصحيحة).</span><span class="sxs-lookup"><span data-stu-id="1be02-106">Verify that the indicator is correct (no typos in IP/URL, correct action, the correct RBAC groups).</span></span>
- <span data-ttu-id="1be02-107">انتظر ساعتين كحد أدنى بعد إنشاء المؤشر لكي تأخذ في الاعتبار أي زمن قد يكون ممكنا.</span><span class="sxs-lookup"><span data-stu-id="1be02-107">Wait the minimum 2 hours after creating the indicator to take into account any possible latency.</span></span>
- <span data-ttu-id="1be02-108">تأكد من أن النظام (الأنظمة) تم تشغيلها في Microsoft Defender لنقطة النهاية.</span><span class="sxs-lookup"><span data-stu-id="1be02-108">Confirm that the system(s) are onboarded to Microsoft Defender for Endpoint.</span></span>
- <span data-ttu-id="1be02-109">تحقق من أن النظام (الأنظمة) يمكنه التواصل مع السحابة.</span><span class="sxs-lookup"><span data-stu-id="1be02-109">Verify that system(s) can communicate with the Cloud.</span></span>
- <span data-ttu-id="1be02-110">تحقق من تمكين الشاشة الذكية والوصول إليها من خلال الذهاب إلى [موقع الاختبار](https://demo.smartscreen.msft.net).</span><span class="sxs-lookup"><span data-stu-id="1be02-110">Verify that Smartscreen is enabled and reachable by going to the [test site](https://demo.smartscreen.msft.net).</span></span>

## <a name="step-2-troubleshoot-the-potential-issue"></a><span data-ttu-id="1be02-111">الخطوة 2: استكشاف المشكلة المحتملة وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="1be02-111">Step 2: Troubleshoot the potential issue</span></span>

- <span data-ttu-id="1be02-112">تأكد من أن العميل يلبي المتطلبات.</span><span class="sxs-lookup"><span data-stu-id="1be02-112">Make sure the client meets the requirements.</span></span> <span data-ttu-id="1be02-113">للحصول على التفاصيل، راجع [إنشاء مؤشرات ل IPs وURLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span><span class="sxs-lookup"><span data-stu-id="1be02-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>
- <span data-ttu-id="1be02-114">تأكد من تشغيل الإصدار الأخير من مستعرض Edge.</span><span class="sxs-lookup"><span data-stu-id="1be02-114">Make sure you're running the latest version of the Edge browser.</span></span> <span data-ttu-id="1be02-115">لمعرفة الإصدار الأخير، راجع معرفة أي إصدار من Microsoft Edge [لديك](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span><span class="sxs-lookup"><span data-stu-id="1be02-115">To find out the latest version, see [Find out which version of Microsoft Edge you have](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span></span>
- <span data-ttu-id="1be02-116">أعد تشغيل مستعرض Edge.</span><span class="sxs-lookup"><span data-stu-id="1be02-116">Restart the Edge browser.</span></span>
- <span data-ttu-id="1be02-117">انتقل إلى الموقع الذي قمت بإعداد مؤشر له.</span><span class="sxs-lookup"><span data-stu-id="1be02-117">Navigate to the site for which you have setup an indicator.</span></span> <span data-ttu-id="1be02-118">إذا لم يظهر الموقع كما هو متوقع، فتابع إلى الخطوة 3.</span><span class="sxs-lookup"><span data-stu-id="1be02-118">If the site does not appear as expected, continue to Step 3.</span></span> 

## <a name="step-3-collect-data"></a><span data-ttu-id="1be02-119">الخطوة 3: تجميع البيانات</span><span class="sxs-lookup"><span data-stu-id="1be02-119">Step 3: Collect data</span></span>

- <span data-ttu-id="1be02-120">تجميع **بيانات MDEClientAnalyzer** التشخيصية.</span><span class="sxs-lookup"><span data-stu-id="1be02-120">Collect **MDEClientAnalyzer** diagnostic data.</span></span> <span data-ttu-id="1be02-121">للحصول على الإرشادات، راجع المشاكل المتعلقة [بآلات التكوين في Microsoft Defender لنقطة النهاية](issues-with-onboarding-machines.md).</span><span class="sxs-lookup"><span data-stu-id="1be02-121">For instructions, see [Issues with onboarding machines to Microsoft Defender for Endpoint](issues-with-onboarding-machines.md).</span></span>
- <span data-ttu-id="1be02-122">إذا كنت مرتاحا لتثبيت تتبع Fiddler وجمعه، فشاهد [Telerik Fiddler](http://www.telerik.com/fiddler).</span><span class="sxs-lookup"><span data-stu-id="1be02-122">If you are comfortable installing and collecting a Fiddler trace, see [Telerik Fiddler](http://www.telerik.com/fiddler).</span></span>
- <span data-ttu-id="1be02-123">إذا كنت تفضل الحصول على إرشادات من دعم Microsoft، فحدد أيقونة الدعم أدناه لفتح حالة دعم.</span><span class="sxs-lookup"><span data-stu-id="1be02-123">If you prefer guidance from Microsoft Support, select the Support icon below to open a support case.</span></span>
