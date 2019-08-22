---
title: مشكلات الاتصال مصمم SharePoint
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: a4aeaeaea5743c276b907c78317ff30f5610be81
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36508410"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="ab645-102">مشكلات الاتصال مصمم SharePoint</span><span class="sxs-lookup"><span data-stu-id="ab645-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="ab645-103">إذا كان SharePoint Designer يواجه مشكلات الاتصال بمواقع SharePoint، حاول الحلول العامة التالية.</span><span class="sxs-lookup"><span data-stu-id="ab645-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="ab645-104">الخطوة 1: التحقق من أنه يتم تحديث 2013 مصمم SharePoint باستخدام [مصمم SharePoint Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) [2 آب/أغسطس عام 2016 تحديث ل 2013 مصمم SharePoint](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="ab645-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="ab645-105">الخطوة 2: مسح ملفات ذاكرة التخزين المؤقت المحلية:</span><span class="sxs-lookup"><span data-stu-id="ab645-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="ab645-106">إغلاق 2013 مصمم SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ab645-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="ab645-107">على الكمبيوتر المحلي، بإزالة كافة الملفات الموجودة في كل مجلد من المجلدات التالية.</span><span class="sxs-lookup"><span data-stu-id="ab645-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="ab645-108">Extensions\Cache خادم %APPDATA%\Microsoft\Web</span><span class="sxs-lookup"><span data-stu-id="ab645-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="ab645-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="ab645-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="ab645-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="ab645-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="ab645-111">افتح 2013 مصمم SharePoint وأدخل حساب مرة أخرى لمعرفة ما إذا كان يعمل.</span><span class="sxs-lookup"><span data-stu-id="ab645-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="ab645-112">الخطوة 3: [تمكين مصادقة 2013 Office على Windows الأجهزة الحديثة](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="ab645-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="ab645-113">الخطوة 4: المسؤولين ستحتاج إلى **السماح لبرنامج نصي مخصص** في إعدادات مركز مسؤول SharePoint للسماح باتصال SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="ab645-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="ab645-114">راجع [السماح أو منع البرامج النصية المخصصة](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) لمزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="ab645-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


