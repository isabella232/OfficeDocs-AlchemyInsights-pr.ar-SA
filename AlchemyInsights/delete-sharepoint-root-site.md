---
title: حذف موقع SharePoint الجذر
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003017"
- "5727"
ms.openlocfilehash: d33029b6fe333b38cee7dba66ba4a5044248f174
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713252"
---
# <a name="delete-the-sharepoint-root-site"></a><span data-ttu-id="e0b36-102">حذف موقع SharePoint الجذر</span><span class="sxs-lookup"><span data-stu-id="e0b36-102">Delete the SharePoint root site</span></span>

<span data-ttu-id="e0b36-103">إن حذف موقع SharePoint الجذر  **غير معتمد.**</span><span class="sxs-lookup"><span data-stu-id="e0b36-103">Deleting the SharePoint root site is  **not supported.**</span></span>

1.  <span data-ttu-id="e0b36-104">إذا تم حذف الموقع الجذر بالفعل، سيختبر المستخدمون الخطأ 404 File Not Found عند محاولة الوصول إلى الموقع.</span><span class="sxs-lookup"><span data-stu-id="e0b36-104">If the root site has already been deleted, users will experience a  404 File Not Found  error when trying to access the site.</span></span>
2.  <span data-ttu-id="e0b36-105">لحل هذه المشكلة، يمكنك استعادة الموقع من مركز [](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) إدارة SharePoint الجديد من خلال الذهاب إلى صفحة "المواقع المحذوفة"، وحدد الموقع الجذر وانقر فوق "استعادة".</span><span class="sxs-lookup"><span data-stu-id="e0b36-105">To resolve, restore the site  from the new SharePoint admin center by going to the  [Deleted sites](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true)  page, select the root site and click  Restore.</span></span>
3.  <span data-ttu-id="e0b36-106">بدلا من حذف الموقع الجذر، استخدم موقع الاستبدال من مركز إدارة SharePoint الجديد بمجرد استعادة الموقع الجذر. [](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site)</span><span class="sxs-lookup"><span data-stu-id="e0b36-106">Instead of deleting the root site, use [replace site](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site)  from the new SharePoint Admin Center once the root site is restored.</span></span>

<span data-ttu-id="e0b36-107">لمزيد من المعلومات، راجع ["تحديث الموقع الجذر"](https://docs.microsoft.com/sharepoint/modern-root-site)</span><span class="sxs-lookup"><span data-stu-id="e0b36-107">For more info, see [Modernize your root site](https://docs.microsoft.com/sharepoint/modern-root-site)</span></span>