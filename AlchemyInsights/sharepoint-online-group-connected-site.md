---
title: أضافه مجموعه إلى موقع SharePoint
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
ms.openlocfilehash: 14ad9dd094902c85eaf0398c76003cea20ad4c0a
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051088"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="f9212-102">المشكلات عند إنشاء أو تجميع المواقع المتصلة في SharePoint علي الإنترنت</span><span class="sxs-lookup"><span data-stu-id="f9212-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="f9212-103">هناك بعض المشكلات الشائعة التي تمت مواجهتها عند إنشاء أو أعاده إنشاء موقع متصل بالمجموعة.</span><span class="sxs-lookup"><span data-stu-id="f9212-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="f9212-104">إذا قمت بحذف مجموعه وموقعها المتصل وترغب في إنشاء موقع آخر بنفس عنوان URL ، ستحتاج إلى أزاله الموقع السابق بشكل دائم.</span><span class="sxs-lookup"><span data-stu-id="f9212-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="f9212-105">تحميل [أداره البرامج الاستراتيجي شل](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="f9212-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="f9212-106">لمزيد من المعلومات حول الشروع في التشغيل مع powershell ، راجع الشروع [في التشغيل باستخدام Shell أداره SharePoint علي الإنترنت](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="f9212-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="f9212-107">أزاله الموقع من المواقع المحذوفة باستخدام cmdlet powershell [أزاله سبوديليدموقع](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="f9212-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="f9212-108">إذا كنت تقوم بإنشاء موقع متصل بمجموعه وتتلقي تحذيرا توجد مجموعه أخرى بنفس الاسم المستعار بالفعل ، تحقق من المجموعات الموجودة من [Office 365 من مركز الاداره](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="f9212-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="f9212-109">لحل هذه المشكلة ، احذف المجموعة الموجودة إذا لم تعد هناك حاجه اليها أو قم بإنشاء الموقع باسم مستعار مختلف معين.</span><span class="sxs-lookup"><span data-stu-id="f9212-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="f9212-110">هناك طرق مختلفه لإنشاء واستخدام المجموعات الحديثة مع SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f9212-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="f9212-111">يمكنك توصيل المواقع الموجودة إلى مجموعه 365 Office.</span><span class="sxs-lookup"><span data-stu-id="f9212-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="f9212-112">لمزيد من المعلومات ، راجع [توصيل مجموعه 365 Office باستخدام الواجهة المستخدمة ل SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="f9212-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="f9212-113">لإنشاء موقع متصل بمجموعه Office 365 ، ستحتاج إلى إنشاء موقع فريق.</span><span class="sxs-lookup"><span data-stu-id="f9212-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="f9212-114">لمزيد من المعلومات ، راجع [إنشاء موقع فريق في SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="f9212-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

