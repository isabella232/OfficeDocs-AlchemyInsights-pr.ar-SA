---
title: إضافة مجموعة إلى موقع SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: e7bfabe1555bb94e915f8544d460deecce6171be
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770338"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="50eee-102">المشكلات عند إنشاء موقع متصل بمجموعة في SharePoint</span><span class="sxs-lookup"><span data-stu-id="50eee-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="50eee-103">تواجه بعض المشكلات الشائعة عند إنشاء موقع متصل بمجموعة أو إعادة إنشائه.</span><span class="sxs-lookup"><span data-stu-id="50eee-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="50eee-104">إذا قمت بحذف مجموعة وموقعمتصل بها وترغب في إنشاء موقع آخر بنفس عنوان URL، فستحتاج إلى إزالة الموقع السابق نهائيًا.</span><span class="sxs-lookup"><span data-stu-id="50eee-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="50eee-105">تحميل [SPO إدارة شل](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="50eee-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="50eee-106">لمزيد من المعلومات حول البدء باستخدام Powershell، راجع [البدء باستخدام SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="50eee-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="50eee-107">إزالة الموقع من المواقع المحذوفة باستخدام [إزالة-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span><span class="sxs-lookup"><span data-stu-id="50eee-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="50eee-108">مطلوب Powershell لحذف مواقع المجموعة بشكل دائم.</span><span class="sxs-lookup"><span data-stu-id="50eee-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="50eee-109">إذا كنت تقوم بإنشاء موقع متصل بمجموعة وتتلقى تحذيرًا: **توجد بالفعل مجموعة أخرى تحمل نفس الاسم المستعار**، فتحقق من المجموعات الموجودة من Office [365 من مركز الإدارة](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="50eee-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="50eee-110">لحل المشكلة، احذف المجموعة الموجودة إذا لم تعد هناك حاجة إليها أو قم بإنشاء الموقع باسم مستعار مختلف معين.</span><span class="sxs-lookup"><span data-stu-id="50eee-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="50eee-111">هناك طرق مختلفة لإنشاء واستخدام المجموعات الحديثة باستخدام SharePoint.</span><span class="sxs-lookup"><span data-stu-id="50eee-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="50eee-112">يمكنك توصيل المواقع الموجودة بمجموعة Office 365.</span><span class="sxs-lookup"><span data-stu-id="50eee-112">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="50eee-113">لمزيد من المعلومات، راجع [توصيل مجموعة Office 365 باستخدام واجهة مستخدم SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="50eee-113">For more info, see [Connect an Office 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="50eee-114">لإنشاء موقع متصل بمجموعة Office 365، ستحتاج إلى إنشاء [موقع فريق](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="50eee-114">To create an Office 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
