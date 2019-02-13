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
ms.openlocfilehash: 20b538846997c021b6e88596a1e8aff401ea935b
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29900851"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="98658-102">إصلاح مشكلة في مشاركة محتوى SharePoint مع المستخدمين الخارجيين</span><span class="sxs-lookup"><span data-stu-id="98658-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="98658-103">تأكد من المشاركة الخارجية قيد التشغيل للمؤسسة الخاصة بك:</span><span class="sxs-lookup"><span data-stu-id="98658-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="98658-104">انتقل إلى [خدمات &amp; صفحة الوظائف الإضافية في مركز مسؤول Office 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)، انقر فوق **مواقع**.</span><span class="sxs-lookup"><span data-stu-id="98658-104">Go to the [Services &amp; add-ins page in the Office 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="98658-p101">تأكد من تشغيل "الإعداد" إلى "على." إذا كان محدداً "الوحيدة القائمة المستخدمين الخارجيين"، تأكد من أن المستخدم الخارجي في مركز مسؤول Office 365.</span><span class="sxs-lookup"><span data-stu-id="98658-p101">Make sure the setting is turned to "On." If "Only existing external users" is selected, make sure the external user is listed in the Office 365 admin center.</span></span>
    
<span data-ttu-id="98658-p102">تأكد من تشغيل الخارجية مشاركته للموقع. لمجموعة موقع التقليدية:</span><span class="sxs-lookup"><span data-stu-id="98658-p102">Make sure external sharing it turned on for the site. For a classic site collection:</span></span>
  
1. <span data-ttu-id="98658-109">في مركز مسؤول SharePoint التقليدية، في الجزء الأيمن، انقر فوق **مجموعات الموقع**.</span><span class="sxs-lookup"><span data-stu-id="98658-109">In the classic SharePoint admin center, in the left pane, click **site collections**.</span></span>
    
2. <span data-ttu-id="98658-110">تحديد الموقع أو المواقع، وعلى "الشريط"، انقر فوق **مشاركة**.</span><span class="sxs-lookup"><span data-stu-id="98658-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="98658-111">موقع فريق ينتمي إلى مجموعة Office 365، أو موقع اتصال:</span><span class="sxs-lookup"><span data-stu-id="98658-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="98658-p103">من هذه الأنواع الجديدة من موقع نفس المشاركة الإعداد كإعداد المؤسسة الخاصة بك، ما لم يسمح الإعداد على نطاق المنظمة لمشاركة الملفات باستخدام الارتباطات التي لا تتطلب تسجيل الدخول. في هذه الحالة، تسمح المواقع المشاركة مع الجديدة والقائمة المستخدمين الخارجيين الذي قام بتسجيل الدخول. لتغيير الإعداد لمواقع محددة، استخدم مركز مسؤول SharePoint جديدة (المعاينة) أو PowerShell. [التعرف على المزيد](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="98658-p103">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in. In this case, the sites allow sharing with new and existing external users who sign in. To change the setting for specific sites, use the new SharePoint admin center (preview) or PowerShell. [Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="98658-116">يمكن إعداد المشاركة الخارجية لأي موقع أكثر تعقيداً من إعدادات المؤسسة، لكن ليس أكثر تساهﻻ من إعداد المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="98658-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

