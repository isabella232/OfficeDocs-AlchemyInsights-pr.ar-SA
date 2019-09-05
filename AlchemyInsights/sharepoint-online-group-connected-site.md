---
title: إضافة مجموعة إلى موقع SharePoint
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 423db4e5bbb85e75aee3548d5b6b46a64ebc6fa0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750507"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="15f7c-102">المشكلات عند إنشاء أو تجميع المواقع المتصلة في SharePoint على الإنترنت</span><span class="sxs-lookup"><span data-stu-id="15f7c-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="15f7c-103">هناك عدد من المشكلات الشائعة التي تمت مواجهتها عند إنشاء موقع متصل بالمجموعة أو إعادة إنشائه.</span><span class="sxs-lookup"><span data-stu-id="15f7c-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="15f7c-104">إذا حذفت مجموعة وموقعها المتصل وترغب في إنشاء موقع آخر بنفس عنوان URL، فستحتاج إلى إزالة الموقع السابق نهائيًا.</span><span class="sxs-lookup"><span data-stu-id="15f7c-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="15f7c-105">تحميل [SPO إدارة شل](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="15f7c-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="15f7c-106">لمزيد من المعلومات حول الشروع في العمل باستخدام powershell، راجع [الشروع في العمل باستخدام SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="15f7c-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="15f7c-107">إزالة الموقع من المواقع المحذوفة باستخدام cmdlet powershell [إزالة SPODeletedSite.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="15f7c-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="15f7c-108">إذا كنت تقوم بإنشاء موقع متصل بمجموعة وتتلقى تحذيرًا، توجد بالفعل مجموعة أخرى بنفس الاسم المستعار، فتحقق من المجموعات الموجودة من [Office 365 من مركز المسؤول](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="15f7c-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="15f7c-109">لحل هذه المشكلة، احذف المجموعة الموجودة إذا لم تعد هناك حاجة إليها أو قم بإنشاء الموقع باسم مستعار مختلف تم تعيينه.</span><span class="sxs-lookup"><span data-stu-id="15f7c-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="15f7c-110">هناك طرق مختلفة لإنشاء واستخدام المجموعات الحديثة مع SharePoint.</span><span class="sxs-lookup"><span data-stu-id="15f7c-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="15f7c-111">يمكنك توصيل المواقع الموجودة بمجموعة Office 365.</span><span class="sxs-lookup"><span data-stu-id="15f7c-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="15f7c-112">لمزيد من المعلومات، راجع [توصيل مجموعة Office 365 باستخدام مستخدم SharePoint ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="15f7c-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="15f7c-113">لإنشاء موقع متصل بمجموعة Office 365، ستحتاج إلى إنشاء موقع فريق.</span><span class="sxs-lookup"><span data-stu-id="15f7c-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="15f7c-114">لمزيد من المعلومات، راجع [إنشاء موقع فريق في SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="15f7c-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

