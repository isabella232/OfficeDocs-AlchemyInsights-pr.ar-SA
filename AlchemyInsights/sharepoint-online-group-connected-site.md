---
title: أضافه مجموعه إلى موقع SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771186"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="32c7c-102">مشاكل عند إنشاء موقع متصل بمجموعه في SharePoint</span><span class="sxs-lookup"><span data-stu-id="32c7c-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="32c7c-103">واجهت بعض المشاكل الشائعة عند إنشاء موقع المجموعة المتصلة أو أعاده إنشائه.</span><span class="sxs-lookup"><span data-stu-id="32c7c-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="32c7c-104">إذا قمت بحذف مجموعه وموقعها المتصل وترغب في إنشاء موقع آخر باستخدام عنوان URL نفسه ، ستحتاج إلى أزاله الموقع السابق بشكل دائم.</span><span class="sxs-lookup"><span data-stu-id="32c7c-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="32c7c-105">تنزيل [Shell لأداره SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="32c7c-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="32c7c-106">للحصول علي مزيد من المعلومات حول بدء استخدام Powershell ، راجع [بدء استخدام SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="32c7c-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="32c7c-107">أزاله الموقع من المواقع [المحذوفة](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) باستخدام الأمرين سبوديليتيدسيتي Powershell cmdlet.</span><span class="sxs-lookup"><span data-stu-id="32c7c-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="32c7c-108">يجب ان تحذف Powershell مواقع المجموعات بشكل دائم.</span><span class="sxs-lookup"><span data-stu-id="32c7c-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="32c7c-109">إذا كنت تقوم بإنشاء موقع متصل بالمجموعة وتلقيت تحذيرا: **هناك مجموعه أخرى تحمل نفس الاسم المستعار موجودة بالفعل**، فتحقق من المجموعات الموجودة من [مركز أداره Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="32c7c-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="32c7c-110">لحل هذه المشكلة ، احذف المجموعة الموجودة إذا لم تعد بحاجه اليها أو أنشئ الموقع باسم مستعار مختلف معين.</span><span class="sxs-lookup"><span data-stu-id="32c7c-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="32c7c-111">هناك طرق مختلفه لإنشاء المجموعات الحديثة واستخدامها مع SharePoint.</span><span class="sxs-lookup"><span data-stu-id="32c7c-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="32c7c-112">يمكنك توصيل مواقع موجودة بمجموعه Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="32c7c-112">You can connect existing sites to a Microsoft 365 group.</span></span> <span data-ttu-id="32c7c-113">لمزيد من المعلومات ، راجع [الاتصال بمجموعه Microsoft 365 باستخدام واجهه مستخدم SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="32c7c-113">For more info, see [Connect a Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="32c7c-114">لإنشاء موقع Microsoft 365 المتصل بالمجموعة ، ستحتاج إلى إنشاء [موقع فريق](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="32c7c-114">To create a Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
