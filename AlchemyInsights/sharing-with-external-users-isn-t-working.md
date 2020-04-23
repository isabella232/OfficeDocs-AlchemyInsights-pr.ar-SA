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
ms.openlocfilehash: 285535d6144825f0935bf72579a483260c2f2bd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767236"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="0f10f-102">إصلاح مشاكل مشاركة محتوى SharePoint مع مستخدمين خارجيين</span><span class="sxs-lookup"><span data-stu-id="0f10f-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="0f10f-103">تأكد من تشغيل المشاركة الخارجية لمؤسستك:</span><span class="sxs-lookup"><span data-stu-id="0f10f-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="0f10f-104">انتقل إلى [ &amp; صفحة الوظائف الإضافية للخدمات في مركز إدارة Microsoft 365،](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)وانقر على **المواقع**.</span><span class="sxs-lookup"><span data-stu-id="0f10f-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="0f10f-105">تأكد من تشغيل الإعداد إلى "تشغيل".</span><span class="sxs-lookup"><span data-stu-id="0f10f-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="0f10f-106">في حالة تحديد "المستخدمين الخارجيين الموجودين فقط"، تأكد من إدراج المستخدم الخارجي في مركز إدارة Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0f10f-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="0f10f-107">تأكد من تشغيل المشاركة الخارجية للموقع.</span><span class="sxs-lookup"><span data-stu-id="0f10f-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="0f10f-108">لمجموعة مواقع كلاسيكية:</span><span class="sxs-lookup"><span data-stu-id="0f10f-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="0f10f-109">في مركز مسؤول SharePoint الجديد، في الجزء الأيسر، انقر فوق **المواقع**.</span><span class="sxs-lookup"><span data-stu-id="0f10f-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="0f10f-110">حدد الموقع أو المواقع، وعلى الشريط، انقر فوق **مشاركة**.</span><span class="sxs-lookup"><span data-stu-id="0f10f-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="0f10f-111">لموقع فريق ينتمي إلى مجموعة Office 365 أو موقع اتصال:</span><span class="sxs-lookup"><span data-stu-id="0f10f-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="0f10f-112">تحتوي أنواع المواقع الجديدة هذه على نفس إعداد المشاركة مثل الإعداد على مستوى المؤسسة، ما لم يسمح الإعداد على مستوى المؤسسة بمشاركة الملفات باستخدام ارتباطات لا تتطلب تسجيل الدخول.</span><span class="sxs-lookup"><span data-stu-id="0f10f-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="0f10f-113">في هذه الحالة، تسمح المواقع بالمشاركة مع المستخدمين الخارجيين الجدد والحاليين الذين يقومون بتسجيل الدخول.</span><span class="sxs-lookup"><span data-stu-id="0f10f-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="0f10f-114">لتغيير الإعداد لمواقع معينة، استخدم مركز مسؤول SharePoint الجديد أو PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0f10f-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="0f10f-115">[تعرّف على المزيد](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="0f10f-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="0f10f-116">يمكن أن يكون إعداد المشاركة الخارجية لأي موقع أكثر تقييداً من الإعداد على مستوى المؤسسة، ولكنه ليس أكثر تساهلاً من الإعداد على مستوى المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="0f10f-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

