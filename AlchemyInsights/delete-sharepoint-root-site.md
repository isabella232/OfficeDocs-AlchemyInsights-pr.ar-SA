---
title: حذف موقع جذر SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003017"
- "5727"
ms.openlocfilehash: 849c5c58ab4688130d71baffac8fe39eddf92f18
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815458"
---
# <a name="delete-the-sharepoint-root-site"></a><span data-ttu-id="6a6ee-102">حذف موقع جذر SharePoint</span><span class="sxs-lookup"><span data-stu-id="6a6ee-102">Delete the SharePoint root site</span></span>

<span data-ttu-id="6a6ee-103">حذف موقع جذر SharePoint **غير مدعوم.**</span><span class="sxs-lookup"><span data-stu-id="6a6ee-103">Deleting the SharePoint root site is  **not supported.**</span></span>

1.  <span data-ttu-id="6a6ee-104">إذا تم حذف موقع الجذر بالفعل، فسيواجه المستخدمون خطأ 404 لم يتم العثور على الملف عند محاولة الوصول إلى الموقع.</span><span class="sxs-lookup"><span data-stu-id="6a6ee-104">If the root site has already been deleted, users will experience a  404 File Not Found  error when trying to access the site.</span></span>
2.  <span data-ttu-id="6a6ee-105">لحل المشكلة، قم باستعادة الموقع من مركز إدارة SharePoint الجديد بالانتقال إلى صفحة [المواقع المحذوفة](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true)، وحدد الموقع الجذر وانقر فوق استعادة.</span><span class="sxs-lookup"><span data-stu-id="6a6ee-105">To resolve, restore the site  from the new SharePoint admin center by going to the  [Deleted sites](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true)  page, select the root site and click  Restore.</span></span>
3.  <span data-ttu-id="6a6ee-106">بدلاً من حذف الموقع الجذر، استخدم [استبدال الموقع](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site) من مركز إدارة SharePoint الجديد بمجرد استعادة الموقع الجذر.</span><span class="sxs-lookup"><span data-stu-id="6a6ee-106">Instead of deleting the root site, use [replace site](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site)  from the new SharePoint Admin Center once the root site is restored.</span></span>

<span data-ttu-id="6a6ee-107">لمزيد من المعلومات، راجع [تحديث الموقع الجذر](https://docs.microsoft.com/sharepoint/modern-root-site)</span><span class="sxs-lookup"><span data-stu-id="6a6ee-107">For more info, see [Modernize your root site](https://docs.microsoft.com/sharepoint/modern-root-site)</span></span>