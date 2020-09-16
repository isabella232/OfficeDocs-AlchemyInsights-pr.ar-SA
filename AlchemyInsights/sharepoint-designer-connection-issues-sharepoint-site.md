---
title: مشاكل الاتصال في SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727158"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="c4307-102">مشاكل الاتصال في SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="c4307-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="c4307-103">إذا واجه SharePoint Designer مشاكل في الاتصال بمواقع SharePoint ، فالرجاء تجربه الحلول الشائعة التالية.</span><span class="sxs-lookup"><span data-stu-id="c4307-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="c4307-104">الخطوة 1: التحقق من تحديث SharePoint Designer 2013 باستخدام [حزمه الخدمة Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) و [2 و 2016 Update ل sharepoint designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="c4307-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="c4307-105">الخطوة 2: مسح ملفات ذاكره التخزين المؤقت المحلية:</span><span class="sxs-lookup"><span data-stu-id="c4307-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="c4307-106">اغلق SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="c4307-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="c4307-107">علي الكمبيوتر المحلي ، قم بازاله كل الملفات التي تم العثور عليها في كل من المجلدات التالية.</span><span class="sxs-lookup"><span data-stu-id="c4307-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="c4307-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="c4307-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="c4307-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="c4307-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="c4307-110">%userprofile%\appdata\local\microsoft\websitecache</span><span class="sxs-lookup"><span data-stu-id="c4307-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="c4307-111">افتح SharePoint Designer 2013 وادخل الحساب مره أخرى لمعرفه ما إذا كان يعمل.</span><span class="sxs-lookup"><span data-stu-id="c4307-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="c4307-112">الخطوة 3: [تمكين المصادقة الحديثة ل Office 2013 علي أجهزه Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="c4307-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>

<span data-ttu-id="c4307-113">الخطوة 4: سيحتاج المسؤولون إلى **السماح بالبرنامج النصي المخصص** في إعدادات مركز أداره sharepoint للسماح باتصال sharepoint Designer.</span><span class="sxs-lookup"><span data-stu-id="c4307-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="c4307-114">راجع [السماح بالبرامج النصية المخصصة أو منع](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) المزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="c4307-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


