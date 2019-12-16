---
title: مشكلات اتصال مصمم SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 9730bd66afd494385db3de605f5fe68d0f274ed3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051700"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="ba490-102">مشكلات اتصال مصمم SharePoint</span><span class="sxs-lookup"><span data-stu-id="ba490-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="ba490-103">إذا كان مصمم SharePoint يواجه مشكلات في الاتصال بمواقع SharePoint ، الرجاء محاولة الحلول الشائعة التالية.</span><span class="sxs-lookup"><span data-stu-id="ba490-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="ba490-104">الخطوة 1: تحقق من ان يتم تحديث SharePoint Designer 2013 مع [Sharepoint مصمم الخدمة Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) و [2 أغسطس 2016 تحديث ل sharepoint designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="ba490-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="ba490-105">الخطوة 2: مسح ملفات ذاكره التخزين المؤقت المحلية:</span><span class="sxs-lookup"><span data-stu-id="ba490-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="ba490-106">إغلاق SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="ba490-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="ba490-107">علي الكمبيوتر المحلي ، قم بازاله كافة الملفات الموجودة في كل من المجلدات التالية.</span><span class="sxs-lookup"><span data-stu-id="ba490-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="ba490-108">%Appdate%\tegs\micscatortontetes\ التخزين المؤقت</span><span class="sxs-lookup"><span data-stu-id="ba490-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="ba490-109">%Appdata%\tedsdesigner\proxyassemblycache \ SharePoint</span><span class="sxs-lookup"><span data-stu-id="ba490-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="ba490-110">%Userprofile%\appdates\locics\mics\websitecache</span><span class="sxs-lookup"><span data-stu-id="ba490-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="ba490-111">فتح SharePoint Designer 2013 وادخل الحساب مره أخرى لمعرفه ما إذا كان يعمل.</span><span class="sxs-lookup"><span data-stu-id="ba490-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="ba490-112">الخطوة 3: [تمكين المصادقة الحديثة ل Office 2013 علي أجهزه Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="ba490-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="ba490-113">الخطوة 4: سيحتاج المسؤولون إلى **السماح بالبرنامج النصي المخصص** في إعدادات مركز مسؤول sharepoint للسماح باتصال مصمم sharepoint.</span><span class="sxs-lookup"><span data-stu-id="ba490-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="ba490-114">راجع [السماح بالبرنامج النصي المخصص أو منعه](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) للحصول علي مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="ba490-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


