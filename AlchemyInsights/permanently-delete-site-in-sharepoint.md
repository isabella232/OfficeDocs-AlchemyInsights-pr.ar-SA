---
title: حذف موقع في SharePoint بشكل دائم
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: 263317339d965d173a5a038fa006e0ce6f8476cc
ms.sourcegitcommit: da04e79b6072321caa16a6ceea6eb5f15de22394
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/25/2020
ms.locfileid: "42955092"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a><span data-ttu-id="1275c-102">حذف موقع في SharePoint بشكل دائم</span><span class="sxs-lookup"><span data-stu-id="1275c-102">Permanently delete a site in SharePoint</span></span>

<span data-ttu-id="1275c-103">لإعادة استخدام عنوان URL من موقع محذوف (لإعادة إنشاء موقع)، أو لحذف موقع نهائياً لأنه لم يعد قيد الاستخدام، يمكنك استخدام **حذف نهائياً** من مركز إدارة SharePoint الجديد.</span><span class="sxs-lookup"><span data-stu-id="1275c-103">To reuse a URL from a deleted site (to recreate a site), or to permanently delete a site because it's no longer in use, you can use **Permanently Delete** from the New SharePoint Admin Center.</span></span> 

1. <span data-ttu-id="1275c-104">انتقل إلى [صفحة المواقع المحذوفة في مركز إدارة SharePoint الجديد](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) وسجّل الدخول باستخدام حساب يحتوي على أذونات المسؤول لمؤسسك.</span><span class="sxs-lookup"><span data-stu-id="1275c-104">Go to the [Deleted sites page of the new SharePoint admin center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) and sign in with an account that has admin permissions for your organization.</span></span> 

2. <span data-ttu-id="1275c-105">من العمود الأيمن، حدد موقعاً.</span><span class="sxs-lookup"><span data-stu-id="1275c-105">In the left column, select a site.</span></span> 

3. <span data-ttu-id="1275c-106">انقر **حذف بشكل دائم**.</span><span class="sxs-lookup"><span data-stu-id="1275c-106">Click **Permanently Delete**.</span></span> 

<span data-ttu-id="1275c-107">**ملاحظة**: لا يمكن حذف المواقع المتصلة بالمجموعة نهائياً من مركز إدارة SharePoint الجديد.</span><span class="sxs-lookup"><span data-stu-id="1275c-107">**Note**: Group-connected sites cannot be permanently deleted from the New SharePoint Admin Center.</span></span> <span data-ttu-id="1275c-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) ستحتاج إلى استخدامه بدلاً من ذلك.</span><span class="sxs-lookup"><span data-stu-id="1275c-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) will need to be used instead.</span></span>  

<span data-ttu-id="1275c-109">للحصول على مزيد من المعلومات، اطلع على [حذف موقع نهائياً](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="1275c-109">For more info, see [Permanently delete a site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span></span> 
