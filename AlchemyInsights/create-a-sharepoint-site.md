---
title: إنشاء موقع SharePoint
ms.author: pebaum
author: todmccoy
ms.audience: Admin
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: e1e71ae9401448ed18058f6307302dcbaf773649
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770842"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="d0346-102">إنشاء موقع SharePoint</span><span class="sxs-lookup"><span data-stu-id="d0346-102">Create a SharePoint site</span></span>

<span data-ttu-id="d0346-103">إنشاء مواقع من [المواقع النشطة](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) في مركز إدارة SharePoint أو إدارتها.</span><span class="sxs-lookup"><span data-stu-id="d0346-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="d0346-104">لمزيد من المعلومات، راجع [إدارة المواقع في مركز مشرف SharePoint الجديد](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="d0346-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="d0346-105">نصائح:</span><span class="sxs-lookup"><span data-stu-id="d0346-105">Tips:</span></span>

- <span data-ttu-id="d0346-106">**لا** يمكنك إنشاء موقع بنفس عنوان URL لموقع موجود.</span><span class="sxs-lookup"><span data-stu-id="d0346-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="d0346-107">إذا قمت بحذف موقع وترغب في إعادة استخدام عنوان URL، فمن المحتمل أن يكون الموقع المحذوف لا يزال موجودًا ضمن [المواقع المحذوفة](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="d0346-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="d0346-108">يجب حذف الموقع نهائيًا لإعادة استخدام عنوان URL.</span><span class="sxs-lookup"><span data-stu-id="d0346-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="d0346-109">لإزالة موقع بالكامل باستخدام Powershell، راجع مثال [إزالة SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet.</span><span class="sxs-lookup"><span data-stu-id="d0346-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="d0346-110">قد لا يتمكن بعض المستخدمين من إنشاء موقع.</span><span class="sxs-lookup"><span data-stu-id="d0346-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="d0346-111">[راجع إدارة إنشاء الموقع في SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="d0346-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="d0346-112">من المحتمل أن يظهر الموقع **عالقًا** في إنشاء لفترة أطول من المتوقع.</span><span class="sxs-lookup"><span data-stu-id="d0346-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="d0346-113">إذا مر أكثر من 24 ساعة منذ أن رأيت هذه المشكلة لأول مرة، يرجى تسجيل تذكرة دعم.</span><span class="sxs-lookup"><span data-stu-id="d0346-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="d0346-114">في كثير من الحالات، نحن نعمل بالفعل على حل.</span><span class="sxs-lookup"><span data-stu-id="d0346-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="d0346-115">يرجى تعطينا ما لا يقل عن 24 ساعة لإكمال الحل.</span><span class="sxs-lookup"><span data-stu-id="d0346-115">Please give us at least 24 hours to complete a solution.</span></span>
