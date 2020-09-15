---
title: استكشاف أخطاء الوصول إلى الرسائل التي تم رفضها
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3550081a12379f73725253214a2c2d44974ab740
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690770"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="edbb8-102">استكشاف أخطاء الوصول إلى الرسائل التي تم رفضها</span><span class="sxs-lookup"><span data-stu-id="edbb8-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="edbb8-103">إذا حصل أحد الأشخاص علي رسالة "رفض الوصول" إلى مجلد مشترك في SharePoint ، فمن المحتمل ان يكون مسؤول مجموعه الموقع قد قام بتمكين "وضع تامين اذن المستخدم بالوصول المحدود".</span><span class="sxs-lookup"><span data-stu-id="edbb8-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="edbb8-104">لإيقاف تشغيل:</span><span class="sxs-lookup"><span data-stu-id="edbb8-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="edbb8-105">استعرض وصولا إلى الموقع ، وانقر فوق الايقونه إعدادات ، ثم انقر فوق **إعدادات الموقع**.</span><span class="sxs-lookup"><span data-stu-id="edbb8-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="edbb8-106">ضمن **أداره مجموعه المواقع المشتركة**، انقر فوق **ميزات مجموعه المواقع المشتركة**.</span><span class="sxs-lookup"><span data-stu-id="edbb8-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="edbb8-107">إلى جانب **وضع تامين اذن المستخدم بالوصول المحدود**، انقر فوق **إلغاء تنشيط**.</span><span class="sxs-lookup"><span data-stu-id="edbb8-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="edbb8-108">كما يمكن ان تظهر رسالة رفض الوصول إلى المجلدات المشتركة إذا كان الموقع عبارة عن موقع نشر.</span><span class="sxs-lookup"><span data-stu-id="edbb8-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="edbb8-109">للحصول علي معلومات ، راجع [رفض الوصول عند الوصول إلى مجلد مشترك](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="edbb8-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="edbb8-110">إذا حصل أحد الأشخاص علي رسالة "رفض الوصول" عند محاولة عرض طلبات الوصول ، فيجب أضافه المستخدم اما كمسؤول مجموعه مواقع مشتركه أو عضو في مجموعه "المالكين" للموقع.</span><span class="sxs-lookup"><span data-stu-id="edbb8-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="edbb8-111">للحصول علي مزيد من المعلومات ، راجع [الوصول مرفوض إلى قائمه طلبات الوصول](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="edbb8-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="edbb8-112">إذا حصل مستخدم علي رسالة "رفض الوصول" بعد ازالتها من Active directory محليا ، ثم تمت اضافتها ، فراجع [الوصول مرفوض عند مزامنة حساب المستخدم إلى Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="edbb8-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

