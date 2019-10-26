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
ms.openlocfilehash: 30c51d84005534cc1de9e8b8136da1a07be57b73
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/25/2019
ms.locfileid: "36738184"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="31346-102">إنشاء موقع SharePoint</span><span class="sxs-lookup"><span data-stu-id="31346-102">Create a SharePoint site</span></span>

<span data-ttu-id="31346-103">يمكنك مشاهده ما يلي للحصول علي معلومات حول إنشاء موقع SharePoint:</span><span class="sxs-lookup"><span data-stu-id="31346-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="31346-104">[أداره المواقع في مركز مسؤول SharePoint الجديد](https://docs.microsoft.com/sharepoint/manage-site-creation): تعرف علي خيارات إنشاء الموقع ، بما في ذلك كيفيه إنشاء موقع كلاسيكي أو موقع فرق لا يتضمن مجموعه 365 Office.</span><span class="sxs-lookup"><span data-stu-id="31346-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="31346-105">[إنشاء موقع فريق في SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): تعرف علي كيفيه إنشاء موقع فريق.</span><span class="sxs-lookup"><span data-stu-id="31346-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Learn how to create a team site.</span></span>
- <span data-ttu-id="31346-106">[إنشاء موقع اتصال في SharePoint علي الإنترنت](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): التعرف علي كيفيه إنشاء موقع اتصالات.</span><span class="sxs-lookup"><span data-stu-id="31346-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="31346-107">[أداره المواقع في مركز مسؤول SharePoint الجديد](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): تعرف علي كيفيه إنشاء موقع كلاسيكي أو موقع فريق لا يتضمن مجموعه 365 Office.</span><span class="sxs-lookup"><span data-stu-id="31346-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> <span data-ttu-id="31346-108">[! نصائح</span><span class="sxs-lookup"><span data-stu-id="31346-108">[!Tips]</span></span>
> - <span data-ttu-id="31346-109">لا يمكنك إنشاء موقع بنفس عنوان URL لموقع موجود.</span><span class="sxs-lookup"><span data-stu-id="31346-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="31346-110">إذا قمت بحذف موقع وكانت ترغب في أعاده استخدام عنوان URL ، فمن الممكن ان يكون الموقع المحذوف لا يزال موجودا ضمن **المواقع المحذوفة**.</span><span class="sxs-lookup"><span data-stu-id="31346-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="31346-111">لأداره المواقع المحذوفة ، راجع [حذف موقع](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="31346-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="31346-112">لأزاله موقع بالبالكامل مع Powershell ، راجع المثال cmdlet [SPSite أزاله](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="31346-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="31346-113">قد لا يتمكن بعض المستخدمين من إنشاء موقع.</span><span class="sxs-lookup"><span data-stu-id="31346-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="31346-114">راجع [أداره إنشاء الموقع في SharePoint علي الإنترنت](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="31346-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="31346-115">من المحتمل ان يظهر الموقع عالقا عند **الإنشاء** لفتره أطول من المتوقع.</span><span class="sxs-lookup"><span data-stu-id="31346-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="31346-116">إذا مرت أكثر من 24 ساعة منذ ان رايت هذه المسالة لأول مره ، يرجى تسجيل تذكره الدعم.</span><span class="sxs-lookup"><span data-stu-id="31346-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="31346-117">في كثير من الحالات ، نحن نعمل بالفعل علي حل.</span><span class="sxs-lookup"><span data-stu-id="31346-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="31346-118">من فضلك أعطنا 24 ساعة علي الأقل لإكمال الحل.</span><span class="sxs-lookup"><span data-stu-id="31346-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="31346-119">إذا كنت بحاجه إلى إنشاء موقع فريق جديد لا يتضمن مجموعه 365 Office ،</span><span class="sxs-lookup"><span data-stu-id="31346-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


