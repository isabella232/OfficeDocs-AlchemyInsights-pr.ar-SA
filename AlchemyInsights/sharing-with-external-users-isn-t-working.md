---
title: المشاركة مع المستخدمين الخارجيين لا يعمل
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 69e290e5a13f40ad045086791189a7d0af88240b
ms.sourcegitcommit: 228c986911ecf73217116a5d1fdcd2e89362774e
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/09/2019
ms.locfileid: "31747585"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="1cd3b-102">إصلاح مشكلة في مشاركة محتوى SharePoint مع المستخدمين الخارجيين</span><span class="sxs-lookup"><span data-stu-id="1cd3b-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="1cd3b-103">تأكد من المشاركة الخارجية قيد التشغيل للمؤسسة الخاصة بك:</span><span class="sxs-lookup"><span data-stu-id="1cd3b-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="1cd3b-104">الانتقال إلى [خدمات &amp; صفحة الوظائف الإضافية في مركز مسؤول Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)، انقر فوق **مواقع**.</span><span class="sxs-lookup"><span data-stu-id="1cd3b-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="1cd3b-105">تأكد من تشغيل "الإعداد" إلى "على."</span><span class="sxs-lookup"><span data-stu-id="1cd3b-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="1cd3b-106">إذا كان محدداً "الوحيدة القائمة المستخدمين الخارجيين"، تأكد من أن المستخدم الخارجي في مركز مسؤول Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1cd3b-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="1cd3b-107">تأكد من تشغيل الخارجية مشاركته للموقع.</span><span class="sxs-lookup"><span data-stu-id="1cd3b-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="1cd3b-108">لمجموعة موقع التقليدية:</span><span class="sxs-lookup"><span data-stu-id="1cd3b-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="1cd3b-109">في مركز مسؤول SharePoint جديد، في الجزء الأيمن، انقر فوق **مواقع**.</span><span class="sxs-lookup"><span data-stu-id="1cd3b-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="1cd3b-110">تحديد الموقع أو المواقع، وعلى "الشريط"، انقر فوق **مشاركة**.</span><span class="sxs-lookup"><span data-stu-id="1cd3b-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="1cd3b-111">موقع فريق ينتمي إلى مجموعة Office 365، أو موقع اتصال:</span><span class="sxs-lookup"><span data-stu-id="1cd3b-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="1cd3b-112">من هذه الأنواع الجديدة من موقع نفس المشاركة الإعداد كإعداد المؤسسة الخاصة بك، ما لم يسمح الإعداد على نطاق المنظمة لمشاركة الملفات باستخدام الارتباطات التي لا تتطلب تسجيل الدخول.</span><span class="sxs-lookup"><span data-stu-id="1cd3b-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="1cd3b-113">في هذه الحالة، تسمح المواقع المشاركة مع الجديدة والقائمة المستخدمين الخارجيين الذي قام بتسجيل الدخول.</span><span class="sxs-lookup"><span data-stu-id="1cd3b-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="1cd3b-114">لتغيير الإعداد لمواقع محددة، استخدم مركز جديد لمسؤول SharePoint أو PowerShell.</span><span class="sxs-lookup"><span data-stu-id="1cd3b-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="1cd3b-115">[التعرف على المزيد](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="1cd3b-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="1cd3b-116">يمكن إعداد المشاركة الخارجية لأي موقع أكثر تعقيداً من إعدادات المؤسسة، لكن ليس أكثر تساهﻻ من إعداد المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="1cd3b-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

