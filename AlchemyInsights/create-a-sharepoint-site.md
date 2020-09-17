---
title: إنشاء موقع SharePoint
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 5ebaa342ca9864bc31a9ef26eebcf42d96523871
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806926"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="7d3cc-102">إنشاء موقع SharePoint</span><span class="sxs-lookup"><span data-stu-id="7d3cc-102">Create a SharePoint site</span></span>

<span data-ttu-id="7d3cc-103">إنشاء مواقع أو ادارتها من [مواقع نشطه](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) في مركز أداره SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7d3cc-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="7d3cc-104">للحصول علي مزيد من المعلومات ، راجع [أداره المواقع في مركز أداره SharePoint الجديد](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="7d3cc-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="7d3cc-105">المزيد</span><span class="sxs-lookup"><span data-stu-id="7d3cc-105">Tips:</span></span>

- <span data-ttu-id="7d3cc-106">**لا يمكنك** إنشاء موقع باستخدام عنوان URL نفسه لموقع موجود.</span><span class="sxs-lookup"><span data-stu-id="7d3cc-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="7d3cc-107">إذا قمت بحذف موقع واتمني لك أعاده استخدام عنوان URL ، فمن المحتمل ان يكون الموقع المحذوف موجودا ضمن [المواقع المحذوفة](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="7d3cc-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="7d3cc-108">سيحتاج الموقع إلى الحذف بشكل دائم لأعاده استخدام عنوان URL.</span><span class="sxs-lookup"><span data-stu-id="7d3cc-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="7d3cc-109">لأزاله موقع بالبالكامل باستخدام Powershell ، راجع المثال الخاص [بازاله SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet.</span><span class="sxs-lookup"><span data-stu-id="7d3cc-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="7d3cc-110">قد لا يتمكن بعض المستخدمين من إنشاء موقع.</span><span class="sxs-lookup"><span data-stu-id="7d3cc-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="7d3cc-111">[راجع أداره إنشاء الموقع في SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="7d3cc-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="7d3cc-112">من المحتمل ان يظهر الموقع بشكل عالق عند **الإنشاء** أكثر من المتوقع.</span><span class="sxs-lookup"><span data-stu-id="7d3cc-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="7d3cc-113">إذا تم تمرير أكثر من 24 ساعة منذ المرة الاولي التي قمت فيها بمشاهده هذه المشكلة ، يرجى تسجيل تذكره دعم.</span><span class="sxs-lookup"><span data-stu-id="7d3cc-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="7d3cc-114">في حالات كثيره ، نحن نعمل بالفعل علي حل.</span><span class="sxs-lookup"><span data-stu-id="7d3cc-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="7d3cc-115">يرجى تقديم 24 ساعة علي الأقل لإكمال حل.</span><span class="sxs-lookup"><span data-stu-id="7d3cc-115">Please give us at least 24 hours to complete a solution.</span></span>
