---
title: تكوين نقطة النهاية DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 039c8f78c5896b66eab5763fb0bbddd3f0b06f2d
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/03/2020
ms.locfileid: "46554751"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="89ad9-102">تكوين نقطة النهاية DLP</span><span class="sxs-lookup"><span data-stu-id="89ad9-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="89ad9-103">يسمح لك نقطة النهاية لـ Microsoft DLP بتوسيع نطاق إمكانية الحماية والمراقبة لـ DLP إلى المعلومات الحساسة على أجهزة Windows 10.</span><span class="sxs-lookup"><span data-stu-id="89ad9-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="89ad9-104">بعد أن يتم إدخال الأجهزة إلى إدارة الأجهزة، يمكنك إنشاء نُهج DLP لفرض إجراءات الحماية على العناصر.</span><span class="sxs-lookup"><span data-stu-id="89ad9-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="89ad9-105">يمكن استخدام "مستكشف الأنشطة" لمراقبة نشاط العناصر الحساسة.</span><span class="sxs-lookup"><span data-stu-id="89ad9-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="89ad9-106">لمزيد من المعلومات، راجع [تشغيل الأجهزة في إدارة الأجهزة](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="89ad9-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="89ad9-107">للبدء مع نقطة النهاية DLP:</span><span class="sxs-lookup"><span data-stu-id="89ad9-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="89ad9-108">تأكد من حصولك على ترخيص SKU/الاشتراكات المناسب.</span><span class="sxs-lookup"><span data-stu-id="89ad9-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="89ad9-109">لمزيد من المعلومات، راجع [ترخيص SKU/الاشتراكات](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="89ad9-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="89ad9-110">تحقق من الأذونات المطلوبة لتمكين إدارة الجهاز، أو الوصول إلى صفحة التشغيل، أو تشغيل/إيقاف مراقبة الجهاز.</span><span class="sxs-lookup"><span data-stu-id="89ad9-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="89ad9-111">لمزيد من المعلومات، راجع [الأذونات](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="89ad9-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="89ad9-112">الأجهزة على متن الطائرة في إدارة الأجهزة باتباع إجراء الأجهزة على متن الطائرة.</span><span class="sxs-lookup"><span data-stu-id="89ad9-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="89ad9-113">إذا كنت في عداد المفقودين على الجهاز على أساس خيار (معاينة) ضمن **إعدادات**التوافق M365 ، تأكد من أن لديك الترخيص المناسب والأذونات المشار إليها أعلاه.</span><span class="sxs-lookup"><span data-stu-id="89ad9-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="89ad9-114">لمزيد من المعلومات، راجع [أجهزة تشغيل .](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices)</span><span class="sxs-lookup"><span data-stu-id="89ad9-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="89ad9-115">إنشاء نُهج DLP لحماية العناصر الحساسة.</span><span class="sxs-lookup"><span data-stu-id="89ad9-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="89ad9-116">للحصول على معلومات، راجع [سيناريوهات نهج نقطة النهاية DLP](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="89ad9-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="89ad9-117">لمزيد من المعلومات حول نقطة النهاية لـ Microsoft DLP، راجع [معرفة المزيد حول منع فقدان بيانات نقطة النهاية لـ Microsoft 365 (معاينة)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="89ad9-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>