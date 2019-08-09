---
title: إنشاء موقع SharePoint
ms.author: efrene
author: efrene
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: ad1a77b69d2d453dbd3daa304759238b329f96ba
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/09/2019
ms.locfileid: "36269903"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="4577a-102">إنشاء موقع SharePoint</span><span class="sxs-lookup"><span data-stu-id="4577a-102">Create a SharePoint site</span></span>

<span data-ttu-id="4577a-103">يمكنك أن ترى ما يلي للحصول على معلومات حول إنشاء موقع SharePoint:</span><span class="sxs-lookup"><span data-stu-id="4577a-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="4577a-104">[إدارة المواقع في مركز مسؤول SharePoint جديدة](https://docs.microsoft.com/sharepoint/manage-site-creation): التعرف على خيارات إنشاء الموقع، بما في ذلك كيفية إنشاء موقع التقليدية أو موقع فرق تتضمن مجموعة Office 365.</span><span class="sxs-lookup"><span data-stu-id="4577a-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="4577a-105">[إنشاء موقع فريق في SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): تعلم كيفية إنشاء موقع فريق.</span><span class="sxs-lookup"><span data-stu-id="4577a-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Learn how to create a team site.</span></span>
- <span data-ttu-id="4577a-106">[إنشاء موقع اتصال في SharePoint على الإنترنت](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): تعلم كيفية إنشاء موقع اتصالات.</span><span class="sxs-lookup"><span data-stu-id="4577a-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="4577a-107">[إدارة المواقع في مركز مسؤول SharePoint جديدة](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): تعلم كيفية إنشاء موقع التقليدية أو موقع فريق تتضمن مجموعة Office 365.</span><span class="sxs-lookup"><span data-stu-id="4577a-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> [! تلميحات]
> - <span data-ttu-id="4577a-109">لا يمكنك إنشاء موقع باستخدام نفس عنوان URL لموقع موجود.</span><span class="sxs-lookup"><span data-stu-id="4577a-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="4577a-110">إذا حذف موقع والتي ترغب في إعادة استخدام URL، من الممكن حذف الموقع لا يزال موجوداً ضمن **مواقع محذوف**.</span><span class="sxs-lookup"><span data-stu-id="4577a-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="4577a-111">لإدارة حذف المواقع، راجع [حذف موقع](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="4577a-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="4577a-112">لإزالة موقع مع Powershell، راجع المثال cmdlet [إزالة SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="4577a-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="4577a-113">بعض المستخدمين قد لا تتمكن من إنشاء موقع.</span><span class="sxs-lookup"><span data-stu-id="4577a-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="4577a-114">راجع [إنشاء موقع إدارة في SharePoint على الإنترنت](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="4577a-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="4577a-115">من الممكن ظهور الموقع عالقة في **إنشاء** وقتاً أطول من المتوقع.</span><span class="sxs-lookup"><span data-stu-id="4577a-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="4577a-116">لقد مرت أكثر من 24 ساعة منذ أول مرة في هذه المسألة، الرجاء تسجيل دعم تذكرة.</span><span class="sxs-lookup"><span data-stu-id="4577a-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="4577a-117">في كثير من الحالات، الفعل نعمل على إيجاد حل.</span><span class="sxs-lookup"><span data-stu-id="4577a-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="4577a-118">الرجاء إعطاء لنا أربع وعشرين ساعة لإكمال حل.</span><span class="sxs-lookup"><span data-stu-id="4577a-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="4577a-119">إذا كنت تريد إنشاء موقع فريق جديد لا يتضمن مجموعة Office 365</span><span class="sxs-lookup"><span data-stu-id="4577a-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


