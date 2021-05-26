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
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657916"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="0fde0-102">تكوين تفادي فقدان البيانات على الأجهزة</span><span class="sxs-lookup"><span data-stu-id="0fde0-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="0fde0-103">يسمح لك تفادي فقدان البيانات على الأجهزة من Microsoft بتوسيع حماية تفادي فقدان البيانات وقدرة مراقبة المعلومات الحساسة على أجهزة Windows 10.</span><span class="sxs-lookup"><span data-stu-id="0fde0-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="0fde0-104">بعد إلحاق الأجهزة في إدارة الأجهزة، يمكنك إنشاء نُهج DLP لفرض إجراءات الحماية على العناصر.</span><span class="sxs-lookup"><span data-stu-id="0fde0-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="0fde0-105">يمكن استخدام مستكشف النشاط لمراقبة نشاط العناصر الحساسة.</span><span class="sxs-lookup"><span data-stu-id="0fde0-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="0fde0-106">لمزيد من المعلومات، اطلع على [إلحاق الأجهزة في إدارة الأجهزة](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="0fde0-106">For more info, see [Onboarding devices into device management](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="0fde0-107">لبدء استخدام تفادي فقدان البيانات على الأجهزة:</span><span class="sxs-lookup"><span data-stu-id="0fde0-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="0fde0-108">تأكد من حصولك على ترخيص SKU/الاشتراكات المناسبة.</span><span class="sxs-lookup"><span data-stu-id="0fde0-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="0fde0-109">لمزيد من المعلومات، اطلع على [ترخيص SKU/الاشتراكات](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="0fde0-109">For more info, see [SKU/subscriptions licensing](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="0fde0-110">تحقق من الأذونات المطلوبة لتمكين إدارة الجهاز أو الوصول إلى صفحة الإلحاق أو تشغيل/إيقاف مراقبة الجهاز.</span><span class="sxs-lookup"><span data-stu-id="0fde0-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="0fde0-111">للمزيد من المعلومات، اطلع على [الأذونات](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="0fde0-111">For more info, see [Permissions](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="0fde0-112">قم بإلحاق الأجهزة في إدارة الأجهزة باتباع إجراء إلحاق الأجهزة.</span><span class="sxs-lookup"><span data-stu-id="0fde0-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="0fde0-113">لمزيد من المعلومات، اطلع على [إلحاق الأجهزة](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="0fde0-113">For more info, see [Onboarding devices](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="0fde0-114">قم بإنشاء نُهج DLP لحماية العناصر الحساسة الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="0fde0-114">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="0fde0-115">لمزيد من المعلومات، اطلع على [سيناريوهات نهج تفادي فقدان البيانات على الأجهزة](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="0fde0-115">For info, see [Endpoint DLP policy scenarios](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="0fde0-116">لمزيد من المعلومات حول تفادي فقدان البيانات على الأجهزة من Microsoft، اطلع على [تعرّف على المزيد حول تفادي فقدان البيانات على الأجهزة من Microsoft 365 (معاينة)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="0fde0-116">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="0fde0-117">**خطوات مهمة لجمع البيانات، إذا كان الدعم مطلوباً:**</span><span class="sxs-lookup"><span data-stu-id="0fde0-117">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="0fde0-118">تنزيل معاينة محلل عميل [MDATP](https://aka.ms/betamdatpanalyzer).</span><span class="sxs-lookup"><span data-stu-id="0fde0-118">Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span></span>
1. <span data-ttu-id="0fde0-119">قم بتشغيل الأداة كمسؤول من نافذة cmd:</span><span class="sxs-lookup"><span data-stu-id="0fde0-119">Run the tool as Admin from the cmd window:</span></span>

    <span data-ttu-id="0fde0-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span><span class="sxs-lookup"><span data-stu-id="0fde0-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span></span>

1. <span data-ttu-id="0fde0-121">عند مطالبتك بإدخال **عدد الدقائق** لتجميع التتبعات: ، أدخل عدد الدقائق المطلوبة لتشغيل السيناريو.</span><span class="sxs-lookup"><span data-stu-id="0fde0-121">When prompted with **Enter the number of minutes to collect traces:**, enter the number of minutes required to run the scenario.</span></span>
1. <span data-ttu-id="0fde0-122">تشغيل السيناريو.</span><span class="sxs-lookup"><span data-stu-id="0fde0-122">Run the scenario.</span></span>

<span data-ttu-id="0fde0-123">جمع إخراج ملف Zip لتقديمه إلى وكيل الدعم.</span><span class="sxs-lookup"><span data-stu-id="0fde0-123">Collect the Zip file output to give to the Support agent.</span></span>
