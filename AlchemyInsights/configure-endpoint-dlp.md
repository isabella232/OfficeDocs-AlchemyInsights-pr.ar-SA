---
title: تكوين تفادي فقدان البيانات على الأجهزة
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402398"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="914e6-102">تكوين تفادي فقدان البيانات على الأجهزة</span><span class="sxs-lookup"><span data-stu-id="914e6-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="914e6-103">يسمح لك تفادي فقدان البيانات على الأجهزة من Microsoft بتوسيع حماية تفادي فقدان البيانات وقدرة مراقبة المعلومات الحساسة على أجهزة Windows 10.</span><span class="sxs-lookup"><span data-stu-id="914e6-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="914e6-104">بعد إلحاق الأجهزة في إدارة الأجهزة، يمكنك إنشاء نُهج DLP لفرض إجراءات الحماية على العناصر.</span><span class="sxs-lookup"><span data-stu-id="914e6-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="914e6-105">يمكن استخدام مستكشف النشاط لمراقبة نشاط العناصر الحساسة.</span><span class="sxs-lookup"><span data-stu-id="914e6-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="914e6-106">لمزيد من المعلومات، اطلع على [إلحاق الأجهزة في إدارة الأجهزة](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="914e6-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="914e6-107">لبدء استخدام تفادي فقدان البيانات على الأجهزة:</span><span class="sxs-lookup"><span data-stu-id="914e6-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="914e6-108">تأكد من حصولك على ترخيص SKU/الاشتراكات المناسبة.</span><span class="sxs-lookup"><span data-stu-id="914e6-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="914e6-109">لمزيد من المعلومات، اطلع على [ترخيص SKU/الاشتراكات](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="914e6-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="914e6-110">تحقق من الأذونات المطلوبة لتمكين إدارة الجهاز أو الوصول إلى صفحة الإلحاق أو تشغيل/إيقاف مراقبة الجهاز.</span><span class="sxs-lookup"><span data-stu-id="914e6-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="914e6-111">للمزيد من المعلومات، اطلع على [الأذونات](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="914e6-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="914e6-112">قم بإلحاق الأجهزة في إدارة الأجهزة باتباع إجراء إلحاق الأجهزة.</span><span class="sxs-lookup"><span data-stu-id="914e6-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="914e6-113">إذا فقدت خيار "إلحاق الجهاز" (معاينة) ضمن **إعدادات** توافق M365، فتأكد من أن لديك الترخيص والأذونات المناسبة المشار إليها أعلاه.</span><span class="sxs-lookup"><span data-stu-id="914e6-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="914e6-114">لمزيد من المعلومات، اطلع على [إلحاق الأجهزة](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="914e6-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="914e6-115">قم بإنشاء نُهج DLP لحماية العناصر الحساسة الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="914e6-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="914e6-116">لمزيد من المعلومات، اطلع على [سيناريوهات نهج تفادي فقدان البيانات على الأجهزة](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="914e6-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span></span>

<span data-ttu-id="914e6-117">لمزيد من المعلومات حول تفادي فقدان البيانات على الأجهزة من Microsoft، اطلع على [تعرّف على المزيد حول تفادي فقدان البيانات على الأجهزة من Microsoft 365 (معاينة)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="914e6-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="914e6-118">**خطوات مهمة لجمع البيانات، إذا كان الدعم مطلوباً:**</span><span class="sxs-lookup"><span data-stu-id="914e6-118">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="914e6-119">تنزيل MDATP Client Analyzer Preview من [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span><span class="sxs-lookup"><span data-stu-id="914e6-119">Download MDATP Client Analyzer Preview from [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span></span>
2. <span data-ttu-id="914e6-120">قم بتشغيل الأداة كمسؤول من نافذة cmd:</span><span class="sxs-lookup"><span data-stu-id="914e6-120">Run the tool as Admin from the cmd window:</span></span>
3. <span data-ttu-id="914e6-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span><span class="sxs-lookup"><span data-stu-id="914e6-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span></span>
4. <span data-ttu-id="914e6-122">عندما يُطلب منك "إدخال عدد الدقائق لتجميع التتبعات:"، أدخل عدد الدقائق المطلوبة لتشغيل السيناريو</span><span class="sxs-lookup"><span data-stu-id="914e6-122">When prompted with “Enter the number of minutes to collect traces: ", enter the number of minutes that are required to run the scenario</span></span>
5. <span data-ttu-id="914e6-123">تشغيل السيناريو</span><span class="sxs-lookup"><span data-stu-id="914e6-123">Run the scenario</span></span>

<span data-ttu-id="914e6-124">قم بتجميع إخراج ملف Zip ليتم تسليمه إلى وكيل الدعم.</span><span class="sxs-lookup"><span data-stu-id="914e6-124">Collect the Zip file output to be given to the Support agent.</span></span>
