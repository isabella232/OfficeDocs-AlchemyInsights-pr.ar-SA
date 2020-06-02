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
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511531"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="acd6b-102">مشكلات اتصال مصمم SharePoint</span><span class="sxs-lookup"><span data-stu-id="acd6b-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="acd6b-103">إذا كان SharePoint Designer يواجه مشكلات في الاتصال بمواقع SharePoint، فيرجى تجربة الحلول الشائعة التالية.</span><span class="sxs-lookup"><span data-stu-id="acd6b-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="acd6b-104">الخطوة 1: تحقق من تحديث SharePoint Designer 2013 باستخدام [حزمة خدمة مصمم SharePoint 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) وتحديث 2 [أغسطس 2016 لمصمم SharePoint 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="acd6b-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="acd6b-105">الخطوة 2: مسح ملفات ذاكرة التخزين المؤقت المحلية:</span><span class="sxs-lookup"><span data-stu-id="acd6b-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="acd6b-106">إغلاق SharePoint مصمم 2013.</span><span class="sxs-lookup"><span data-stu-id="acd6b-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="acd6b-107">على الكمبيوتر المحلي، قم بإزالة كافة الملفات الموجودة في كل من المجلدات التالية.</span><span class="sxs-lookup"><span data-stu-id="acd6b-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="acd6b-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="acd6b-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="acd6b-109">%APPDATA%\Microsoft\SharePoint مصمم\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="acd6b-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="acd6b-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="acd6b-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="acd6b-111">افتح SharePoint Designer 2013 وأدخل الحساب مرة أخرى لمعرفة ما إذا كان يعمل.</span><span class="sxs-lookup"><span data-stu-id="acd6b-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="acd6b-112">الخطوة 3: [تمكين المصادقة الحديثة لـ Office 2013 على أجهزة Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="acd6b-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>

<span data-ttu-id="acd6b-113">الخطوة 4: سيحتاج المسؤولون إلى **السماح بالبرنامج النصي المخصص** في إعدادات مركز مسؤول SharePoint للسماح باتصال مصمم SharePoint.</span><span class="sxs-lookup"><span data-stu-id="acd6b-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="acd6b-114">راجع [السماح بالبرنامج النصي المخصص أو منعه](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="acd6b-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


