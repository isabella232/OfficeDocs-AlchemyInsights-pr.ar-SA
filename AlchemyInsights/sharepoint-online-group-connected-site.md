---
title: إضافة مجموعة إلى موقع SharePoint
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: f0126f7f753275e9bbf8c3a09a6af5faf9a27862
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758718"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a><span data-ttu-id="18a12-102">إنشاء مجموعة موقع المتصلة في SharePoint عبر إنترنت</span><span class="sxs-lookup"><span data-stu-id="18a12-102">Create group connected site in SharePoint Online</span></span>

<span data-ttu-id="18a12-103">هناك اثنين من المشاكل الشائعة عند إنشاء أو إعادة إنشاء مجموعة الموقع متصلاً.</span><span class="sxs-lookup"><span data-stu-id="18a12-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="18a12-104">إذا قمت بحذف مجموعة والمواقع المتصلة به وترغب في إنشاء موقع آخر باستخدام URL نفسه، سوف تحتاج إلى إزالة الموقع السابق.</span><span class="sxs-lookup"><span data-stu-id="18a12-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="18a12-105">تحميل [Shell إدارة مكتب التخطيط الاستراتيجي](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="18a12-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="18a12-106">لمزيد من المعلومات حول الشروع في العمل مع powershell، راجع [الشروع في استخدام SharePoint Shell إدارة الإنترنت](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="18a12-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="18a12-107">إزالة الموقع من "المواقع المحذوفة" استخدام cmdlet powershell [إزالة سبوديليتيدسيتي](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="18a12-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="18a12-108">إذا كنت تقوم بإنشاء مجموعة موقع متصلة وتلقى تحذير مجموعة أخرى بنفس الاسم المستعار بالفعل، تحقق من مجموعات موجودة من [Office 365 من مركز الإدارة](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="18a12-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="18a12-109">لحل هذه المشكلة أو حذف مجموعة موجودة إذا لم يعد مطلوباً أو إنشاء الموقع باستخدام اسم مستعار مختلف المعينة.</span><span class="sxs-lookup"><span data-stu-id="18a12-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="18a12-110">هناك طرق مختلفة لإنشاء واستخدام مجموعات الحديثة مع SharePoint.</span><span class="sxs-lookup"><span data-stu-id="18a12-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="18a12-111">يمكنك توصيل مواقع موجودة لمجموعة Office 365.</span><span class="sxs-lookup"><span data-stu-id="18a12-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="18a12-112">لمزيد من المعلومات، راجع [الاتصال مجموعة Office 365 استخدام إينيتيرفيس المستخدم SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="18a12-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="18a12-113">لإنشاء موقع متصلة مجموعة Office 365، ستحتاج إلى إنشاء "موقع الفريق".</span><span class="sxs-lookup"><span data-stu-id="18a12-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="18a12-114">لمزيد من المعلومات، راجع [إنشاء موقع فريق في SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="18a12-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

