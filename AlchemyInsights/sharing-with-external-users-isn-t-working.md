---
title: المشاركة مع المستخدمين الخارجيين لا تعمل
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
ms.openlocfilehash: d4c8fc75ff8db2319b88a20bea9b3ee661f2e36e
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/18/2019
ms.locfileid: "36502218"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="bcaeb-102">إصلاح مشكلات مشاركه محتوي SharePoint مع المستخدمين الخارجيين</span><span class="sxs-lookup"><span data-stu-id="bcaeb-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="bcaeb-103">تاكد من تشغيل المشاركة الخارجية للمؤسسة الخاصة بك:</span><span class="sxs-lookup"><span data-stu-id="bcaeb-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="bcaeb-104">انتقل إلى [صفحه الخدمات &amp; الاضافيه في مركز مسؤول Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)، وانقر فوق **مواقع**.</span><span class="sxs-lookup"><span data-stu-id="bcaeb-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="bcaeb-105">تاكد من تشغيل الاعداد إلى "تشغيل".</span><span class="sxs-lookup"><span data-stu-id="bcaeb-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="bcaeb-106">في حاله تحديد "المستخدمين الخارجيين الموجودين فقط" ، تاكد من سرد المستخدم الخارجي في مركز مسؤول Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="bcaeb-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="bcaeb-107">تاكد من المشاركة الخارجية التي تم تشغيلها للموقع.</span><span class="sxs-lookup"><span data-stu-id="bcaeb-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="bcaeb-108">لمجموعه الموقع الكلاسيكية:</span><span class="sxs-lookup"><span data-stu-id="bcaeb-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="bcaeb-109">في مركز مسؤول SharePoint الجديد ، في الجزء الأيمن ، انقر فوق **مواقع**.</span><span class="sxs-lookup"><span data-stu-id="bcaeb-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="bcaeb-110">حدد الموقع أو المواقع ، وعلي الشريط ، انقر فوق **مشاركه**.</span><span class="sxs-lookup"><span data-stu-id="bcaeb-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="bcaeb-111">لموقع الفريق الذي ينتمي إلى مجموعه 365 Office أو موقع اتصال:</span><span class="sxs-lookup"><span data-stu-id="bcaeb-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="bcaeb-112">تحتوي أنواع المواقع الجديدة هذه علي نفس اعداد المشاركة كاعداد علي مستوي المؤسسة ، ما لم يسمح الاعداد علي مستوي المؤسسة بمشاركه الملفات باستخدام الارتباطات التي لا تتطلب تسجيل الدخول.</span><span class="sxs-lookup"><span data-stu-id="bcaeb-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="bcaeb-113">في هذه الحالة ، تسمح المواقع بالمشاركة مع المستخدمين الخارجيين الجدد والحاليين الذين يقومون بتسجيل الدخول.</span><span class="sxs-lookup"><span data-stu-id="bcaeb-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="bcaeb-114">لتغيير الاعداد لمواقع معينه ، استخدم مركز مسؤول SharePoint الجديد أو PowerShell.</span><span class="sxs-lookup"><span data-stu-id="bcaeb-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="bcaeb-115">[تعلم المزيد](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="bcaeb-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="bcaeb-116">يمكن ان يكون اعداد المشاركة الخارجية لأي موقع أكثر تقييدا من الاعداد علي مستوي المؤسسة ، ولكن ليس أكثر تساهلا من الاعداد علي مستوي المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="bcaeb-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

