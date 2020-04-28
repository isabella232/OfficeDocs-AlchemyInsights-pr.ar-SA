---
title: لا تعمل المشاركة مع المستخدمين الخارجيين
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 37da77c73b3abbdcf9cb2b9c4c43f31eea3c0a49
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/27/2020
ms.locfileid: "43912989"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="e5469-102">إصلاح مشاكل مشاركة محتوى SharePoint مع مستخدمين خارجيين</span><span class="sxs-lookup"><span data-stu-id="e5469-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="e5469-103">تأكد من تشغيل المشاركة الخارجية لمؤسستك:</span><span class="sxs-lookup"><span data-stu-id="e5469-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="e5469-104">انتقل إلى [ &amp; صفحة الوظائف الإضافية للخدمات في مركز إدارة Microsoft 365،](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)وانقر على **المواقع**.</span><span class="sxs-lookup"><span data-stu-id="e5469-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="e5469-105">تأكد من تشغيل الإعداد إلى "تشغيل".</span><span class="sxs-lookup"><span data-stu-id="e5469-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="e5469-106">في حالة تحديد "المستخدمين الخارجيين الموجودين فقط"، تأكد من إدراج المستخدم الخارجي في مركز إدارة Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e5469-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="e5469-107">تأكد من تشغيل المشاركة الخارجية للموقع.</span><span class="sxs-lookup"><span data-stu-id="e5469-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="e5469-108">لمجموعة مواقع كلاسيكية:</span><span class="sxs-lookup"><span data-stu-id="e5469-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="e5469-109">في مركز مسؤول SharePoint الجديد، في الجزء الأيسر، انقر فوق **المواقع**.</span><span class="sxs-lookup"><span data-stu-id="e5469-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="e5469-110">حدد الموقع أو المواقع، وعلى الشريط، انقر فوق **مشاركة**.</span><span class="sxs-lookup"><span data-stu-id="e5469-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="e5469-111">لموقع فريق ينتمي إلى مجموعة Microsoft 365 أو موقع اتصال:</span><span class="sxs-lookup"><span data-stu-id="e5469-111">For a team site that belongs to an Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="e5469-112">تحتوي أنواع المواقع الجديدة هذه على نفس إعداد المشاركة مثل الإعداد على مستوى المؤسسة، ما لم يسمح الإعداد على مستوى المؤسسة بمشاركة الملفات باستخدام ارتباطات لا تتطلب تسجيل الدخول.</span><span class="sxs-lookup"><span data-stu-id="e5469-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="e5469-113">في هذه الحالة، تسمح المواقع بالمشاركة مع المستخدمين الخارجيين الجدد والحاليين الذين يقومون بتسجيل الدخول.</span><span class="sxs-lookup"><span data-stu-id="e5469-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="e5469-114">لتغيير الإعداد لمواقع معينة، استخدم مركز مسؤول SharePoint الجديد أو PowerShell.</span><span class="sxs-lookup"><span data-stu-id="e5469-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="e5469-115">[تعرّف على المزيد](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="e5469-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="e5469-116">يمكن أن يكون إعداد المشاركة الخارجية لأي موقع أكثر تقييداً من الإعداد على مستوى المؤسسة، ولكنه ليس أكثر تساهلاً من الإعداد على مستوى المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="e5469-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

