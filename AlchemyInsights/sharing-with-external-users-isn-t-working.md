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
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 4b132a3cb0fac015ab44a1fa08565af15b7e8121
ms.sourcegitcommit: c003a5db7edc3a44fb5b31b46cd45f12b62d172a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/22/2019
ms.locfileid: "30207672"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="2d3a2-102">إصلاح مشكلة في مشاركة محتوى SharePoint مع المستخدمين الخارجيين</span><span class="sxs-lookup"><span data-stu-id="2d3a2-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="2d3a2-103">تأكد من المشاركة الخارجية قيد التشغيل للمؤسسة الخاصة بك:</span><span class="sxs-lookup"><span data-stu-id="2d3a2-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="2d3a2-104">الانتقال إلى [خدمات &amp; صفحة الوظائف الإضافية في مركز مسؤول Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)، انقر فوق **مواقع**.</span><span class="sxs-lookup"><span data-stu-id="2d3a2-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="2d3a2-p101">تأكد من تشغيل "الإعداد" إلى "على." إذا كان محدداً "الوحيدة القائمة المستخدمين الخارجيين"، تأكد من أن المستخدم الخارجي في مركز مسؤول Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2d3a2-p101">Make sure the setting is turned to "On." If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="2d3a2-p102">تأكد من تشغيل الخارجية مشاركته للموقع. لمجموعة موقع التقليدية:</span><span class="sxs-lookup"><span data-stu-id="2d3a2-p102">Make sure external sharing it turned on for the site. For a classic site collection:</span></span>
  
1. <span data-ttu-id="2d3a2-109">في مركز مسؤول SharePoint التقليدية، في الجزء الأيمن، انقر فوق **مجموعات الموقع**.</span><span class="sxs-lookup"><span data-stu-id="2d3a2-109">In the classic SharePoint admin center, in the left pane, click **site collections**.</span></span>
    
2. <span data-ttu-id="2d3a2-110">تحديد الموقع أو المواقع، وعلى "الشريط"، انقر فوق **مشاركة**.</span><span class="sxs-lookup"><span data-stu-id="2d3a2-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="2d3a2-111">موقع فريق ينتمي إلى مجموعة Office 365، أو موقع اتصال:</span><span class="sxs-lookup"><span data-stu-id="2d3a2-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="2d3a2-p103">من هذه الأنواع الجديدة من موقع نفس المشاركة الإعداد كإعداد المؤسسة الخاصة بك، ما لم يسمح الإعداد على نطاق المنظمة لمشاركة الملفات باستخدام الارتباطات التي لا تتطلب تسجيل الدخول. في هذه الحالة، تسمح المواقع المشاركة مع الجديدة والقائمة المستخدمين الخارجيين الذي قام بتسجيل الدخول. لتغيير الإعداد لمواقع محددة، استخدم مركز مسؤول SharePoint جديدة (المعاينة) أو PowerShell. [التعرف على المزيد](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="2d3a2-p103">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in. In this case, the sites allow sharing with new and existing external users who sign in. To change the setting for specific sites, use the new SharePoint admin center (preview) or PowerShell. [Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="2d3a2-116">يمكن إعداد المشاركة الخارجية لأي موقع أكثر تعقيداً من إعدادات المؤسسة، لكن ليس أكثر تساهﻻ من إعداد المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="2d3a2-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

