---
title: إزالة خدمة الخلفية ل Microsoft Search في Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816058"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a><span data-ttu-id="826ae-102">إزالة خدمة الخلفية ل Microsoft Search في Bing</span><span class="sxs-lookup"><span data-stu-id="826ae-102">Remove the background service for Microsoft Search in Bing</span></span>

<span data-ttu-id="826ae-103">لإزالة خدمة الخلفية ل Microsoft Search في Bing، يمكنك تجربة الحلول التالية:</span><span class="sxs-lookup"><span data-stu-id="826ae-103">To remove the background service for Microsoft Search in Bing, you can try the following remedies:</span></span>

1. <span data-ttu-id="826ae-104">لإعادة إعدادات محرك البحث الأصلي، يمكنك القيام بما يلي:</span><span class="sxs-lookup"><span data-stu-id="826ae-104">To revert to the original search engine settings, do the following things:</span></span>

    <span data-ttu-id="826ae-105">أ.</span><span class="sxs-lookup"><span data-stu-id="826ae-105">a.</span></span> <span data-ttu-id="826ae-106">قم **بتبديل مفتاح التبديل [](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) استخدام Bing** كمحرك بحث افتراضي إلى إيقاف التشغيل .</span><span class="sxs-lookup"><span data-stu-id="826ae-106">Switch the **Use Bing as your default search engine [toggle](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Off**.</span></span>

    <span data-ttu-id="826ae-107">ب.</span><span class="sxs-lookup"><span data-stu-id="826ae-107">b.</span></span> <span data-ttu-id="826ae-108">[انتقل إلى مركز إدارة Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) ومسح الإعداد الذي يؤثر على جميع المستخدمين في مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="826ae-108">[Go to the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) and clear the setting that affects all users in your organization.</span></span>

2. <span data-ttu-id="826ae-109">لإزالة خدمة الخلفية من جهاز فردي، قم بالمهام التالية:</span><span class="sxs-lookup"><span data-stu-id="826ae-109">To remove the background service from an individual device, do the following tasks:</span></span>

    <span data-ttu-id="826ae-110">أ.</span><span class="sxs-lookup"><span data-stu-id="826ae-110">a.</span></span> <span data-ttu-id="826ae-111">اختر **لوحة التحكم > البرامج > والبرامج والميزات**.</span><span class="sxs-lookup"><span data-stu-id="826ae-111">Choose **Control Panel > Programs > Programs and Features**.</span></span>

    <span data-ttu-id="826ae-112">ب.</span><span class="sxs-lookup"><span data-stu-id="826ae-112">b.</span></span> <span data-ttu-id="826ae-113">انقر ب زر **الماوس الأيمن فوق بحث Microsoft في Bing** ضمن قائمة البرامج المثبتة، ثم انقر فوق إلغاء **التثبيت.**</span><span class="sxs-lookup"><span data-stu-id="826ae-113">Right-click **Microsoft Search in Bing** under the list of installed programs, and then click **Uninstall**.</span></span>

3. <span data-ttu-id="826ae-114">لإزالة خدمة الخلفية من أجهزة متعددة في مؤسستك، سجل دخولك كمسؤول ثم قم بتشغيل الأمر التالي في برنامج نصي:</span><span class="sxs-lookup"><span data-stu-id="826ae-114">To remove the background service from multiple devices in your organization, log in as an administrator and run the following command in a script:</span></span> 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
