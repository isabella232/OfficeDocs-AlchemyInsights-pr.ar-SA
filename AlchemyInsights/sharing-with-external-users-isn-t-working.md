---
title: المشاركة مع المستخدمين الخارجيين لا يعملون
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691562"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="2607d-102">إصلاح المشاكل المتعلقة بمشاركه محتوي SharePoint مع مستخدمين خارجيين</span><span class="sxs-lookup"><span data-stu-id="2607d-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="2607d-103">تاكد من تشغيل المشاركة الخارجية لمؤسسك:</span><span class="sxs-lookup"><span data-stu-id="2607d-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="2607d-104">انتقل إلى [ &amp; صفحه الوظائف الاضافيه الخاصة بالخدمات في مركز أداره Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)، وانقر فوق **المواقع**.</span><span class="sxs-lookup"><span data-stu-id="2607d-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="2607d-105">تاكد من ان الاعداد في وضع التشغيل.</span><span class="sxs-lookup"><span data-stu-id="2607d-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="2607d-106">إذا تم تحديد "مستخدمين خارجيين فقط" ، فتاكد من ان المستخدم الخارجي مدرج في مركز أداره Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2607d-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="2607d-107">تاكد من تشغيل المشاركة الخارجية للموقع.</span><span class="sxs-lookup"><span data-stu-id="2607d-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="2607d-108">بالنسبة إلى مجموعه المواقع المشتركة التقليدية:</span><span class="sxs-lookup"><span data-stu-id="2607d-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="2607d-109">في مركز أداره SharePoint الجديد ، في الجزء الأيمن ، انقر فوق **المواقع**.</span><span class="sxs-lookup"><span data-stu-id="2607d-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="2607d-110">حدد الموقع أو المواقع ، وعلي الشريط ، انقر فوق **مشاركه**.</span><span class="sxs-lookup"><span data-stu-id="2607d-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="2607d-111">بالنسبة إلى موقع الفريق الذي ينتمي إلى مجموعه Microsoft 365 أو موقع اتصال:</span><span class="sxs-lookup"><span data-stu-id="2607d-111">For a team site that belongs to a Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="2607d-112">تتضمن أنواع المواقع الجديدة هذه إعدادات المشاركة نفسها التي يستخدمها الاعداد علي مستوي المؤسسة ، ما لم يكن الاعداد علي مستوي المؤسسة يسمح بمشاركه الملفات باستخدام الارتباطات التي لا تتطلب تسجيل الدخول.</span><span class="sxs-lookup"><span data-stu-id="2607d-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="2607d-113">في هذه الحالة ، تسمح المواقع بالمشاركة مع المستخدمين الخارجيين الجدد والموجودين الذين قاموا بتسجيل الدخول.</span><span class="sxs-lookup"><span data-stu-id="2607d-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="2607d-114">لتغيير اعداد مواقع معينه ، استخدم مركز أداره SharePoint الجديد أو PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2607d-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="2607d-115">[تعرّف على المزيد](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="2607d-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="2607d-116">يمكن ان يكون اعداد المشاركة الخارجية لأي موقع أكثر تقييدا من الاعداد علي مستوي المؤسسة ، ولكن لا يمكنك القيام بالمزيد من الاتاحه من الاعداد علي مستوي المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="2607d-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

