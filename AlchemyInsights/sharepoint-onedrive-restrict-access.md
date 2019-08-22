---
title: تقييد الوصول في SharePoint أو أندريف
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 84f2d4b6e5fd2380a2fa96e30953c68aab203cd3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559864"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="3b571-102">تقييد الوصول في SharePoint أو أندريف</span><span class="sxs-lookup"><span data-stu-id="3b571-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="3b571-103">هناك العديد من الطرق لتقييد الوصول إلى خدمات عبر الإنترنت/أندريف SharePoint.</span><span class="sxs-lookup"><span data-stu-id="3b571-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="3b571-104">يلي هذه الطرق تقييد وصول مختلف.</span><span class="sxs-lookup"><span data-stu-id="3b571-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="3b571-105">**تقييد الإذن**</span><span class="sxs-lookup"><span data-stu-id="3b571-105">**Permission Restriction**</span></span>

<span data-ttu-id="3b571-106">في SharePoint على الإنترنت وأونيدريفي للعمل، نحن تقييد الوصول إلى عناصر مثل المواقع والملفات والمجلدات بمنح حق الوصول إلى المجموعات/الأفراد الذين ينبغي أن تتاح فقط.</span><span class="sxs-lookup"><span data-stu-id="3b571-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="3b571-107">تخصيص الأذونات لمكتبة أو قائمة SharePoint</span><span class="sxs-lookup"><span data-stu-id="3b571-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="3b571-108">تخصيص أذونات موقع SharePoint</span><span class="sxs-lookup"><span data-stu-id="3b571-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="3b571-109">تغيير الأذونات على مجلد فرعي</span><span class="sxs-lookup"><span data-stu-id="3b571-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="3b571-110">التحكم بالوصول من الأجهزة غير المدارة</span><span class="sxs-lookup"><span data-stu-id="3b571-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="3b571-111">ك SharePoint أو المسؤول العمومي في Office 365، يمكنك حظر أو تقييد الوصول إلى محتوى SharePoint وأندريف من الأجهزة غير المدارة (تلك المختلط الإعلانية المرتبطة أو متوافقة في إينتوني).</span><span class="sxs-lookup"><span data-stu-id="3b571-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="3b571-112">**قيود موقع الشبكة**</span><span class="sxs-lookup"><span data-stu-id="3b571-112">**Network Location Restriction**</span></span>

<span data-ttu-id="3b571-113">كمسؤول تكنولوجيا المعلومات، يمكنك التحكم في الوصول إلى موارد SharePoint وأندريف استناداً إلى شبكة المعرفة المواقع الموثوق بها.</span><span class="sxs-lookup"><span data-stu-id="3b571-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="3b571-114">هذا يعرف أيضا نهج يستند إلى الموقع.</span><span class="sxs-lookup"><span data-stu-id="3b571-114">This is also known as location-based policy.</span></span> <span data-ttu-id="3b571-115">لمزيد من المعلومات، انظر [التحكم في الوصول إلى SharePoint والبيانات أندريف استناداً إلى موقع شبكة الاتصال](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="3b571-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="3b571-116">**قيد تأمين الموقع**</span><span class="sxs-lookup"><span data-stu-id="3b571-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="3b571-117">في SharePoint على الإنترنت لديك القدرة على تأمين مجموعة موقع، حيث لا أحد يملك حق الوصول.</span><span class="sxs-lookup"><span data-stu-id="3b571-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="3b571-118">يتم تعيين هذه عبر PowerShell واستخدام الخاصية-LockState [سبوسيتي مجموعة](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) [SharePoint Shell إدارة الإنترنت](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="3b571-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="3b571-119">**منع المستخدمين من إنشاء المواقع أو المواقع الفرعية**</span><span class="sxs-lookup"><span data-stu-id="3b571-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="3b571-120">كمسؤول SharePoint أو المسؤول العمومي Office 365، يمكنك السماح للمستخدمين بإنشاء وإدارة مواقع SharePoint الخاصة بهم، وتحديد أي نوع من المواقع التي يمكن أن تخلق، ثم عين الموقع المواقع.</span><span class="sxs-lookup"><span data-stu-id="3b571-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="3b571-121">لمزيد من المعلومات، انظر [إنشاء موقع إدارة في SharePoint عبر إنترنت](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="3b571-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

