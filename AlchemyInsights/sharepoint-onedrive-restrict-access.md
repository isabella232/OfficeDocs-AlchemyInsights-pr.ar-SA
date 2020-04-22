---
title: تقييد الوصول في SharePoint أو OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 39aa8cd6e649eca4a1e196eeb589a825364d0977
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692752"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="3115c-102">تقييد الوصول في SharePoint أو OneDrive</span><span class="sxs-lookup"><span data-stu-id="3115c-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="3115c-103">هناك العديد من الطرق لتقييد الوصول إلى خدمات SharePoint Online/OneDrive.</span><span class="sxs-lookup"><span data-stu-id="3115c-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="3115c-104">وفيما يلي طرق تقييد الوصول المختلفة هذه.</span><span class="sxs-lookup"><span data-stu-id="3115c-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="3115c-105">**تقييد الإذن**</span><span class="sxs-lookup"><span data-stu-id="3115c-105">**Permission Restriction**</span></span>

<span data-ttu-id="3115c-106">في SharePoint Online و OneDrive للأعمال، نقيد الوصول إلى عناصر مثل المواقع والملفات والمجلدات من خلال منح حق الوصول فقط إلى تلك المجموعات /الأفراد الذين يجب أن يكون لديهم حق الوصول.</span><span class="sxs-lookup"><span data-stu-id="3115c-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="3115c-107">تخصيص أذونات لقائمة SharePoint أو مكتبة</span><span class="sxs-lookup"><span data-stu-id="3115c-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="3115c-108">تخصيص أذونات موقع SharePoint</span><span class="sxs-lookup"><span data-stu-id="3115c-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="3115c-109">تغيير الأذونات على مجلد فرعي</span><span class="sxs-lookup"><span data-stu-id="3115c-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="3115c-110">التحكم في الوصول من الأجهزة غير المدارة</span><span class="sxs-lookup"><span data-stu-id="3115c-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="3115c-111">كـ SharePoint أو مسؤول عمومي، يمكنك حظر أو تقييد الوصول إلى محتوى SharePoint وOneDrive من الأجهزة غير المدارة (تلك التي لا ينضم إليها الإعلان المختلط أو متوافقمعها في Intune).</span><span class="sxs-lookup"><span data-stu-id="3115c-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="3115c-112">**تقييد موقع الشبكة**</span><span class="sxs-lookup"><span data-stu-id="3115c-112">**Network Location Restriction**</span></span>

<span data-ttu-id="3115c-113">كمسؤول تكنولوجيا المعلومات، يمكنك التحكم في الوصول إلى موارد SharePoint و OneDrive استنادًا إلى مواقع الشبكة المحددة التي تثق بها.</span><span class="sxs-lookup"><span data-stu-id="3115c-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="3115c-114">ويُعرف هذا أيضًا باسم النهج المستند إلى الموقع.</span><span class="sxs-lookup"><span data-stu-id="3115c-114">This is also known as location-based policy.</span></span> <span data-ttu-id="3115c-115">لمزيد من المعلومات، يرجى الاطلاع [على التحكم في الوصول إلى بيانات SharePoint Online و OneDrive استنادًا إلى موقع الشبكة](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="3115c-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="3115c-116">**تقييد قفل الموقع**</span><span class="sxs-lookup"><span data-stu-id="3115c-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="3115c-117">داخل SharePoint Online لديك القدرة على تأمين مجموعة مواقع ، لذلك لا أحد لديه حق الوصول.</span><span class="sxs-lookup"><span data-stu-id="3115c-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="3115c-118">يتم تعيين هذا عبر PowerShell [وSharePoint إدارة الإنترنت شل](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) باستخدام [خاصية Set-SPOSite-LockState.](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="3115c-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="3115c-119">**تقييد المستخدمين من إنشاء مواقع أو مواقع فرعية**</span><span class="sxs-lookup"><span data-stu-id="3115c-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="3115c-120">كمسؤول SharePoint أو مسؤول عالمي، يمكنك السماح للمستخدمين بإنشاء مواقع SharePoint الخاصة بهم وإدارتها، وتحديد نوع المواقع التي يمكنهم إنشاؤها، وتحديد موقع المواقع.</span><span class="sxs-lookup"><span data-stu-id="3115c-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="3115c-121">لمزيد من المعلومات، يرجى [الاطلاع على إدارة إنشاء الموقع في SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="3115c-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

