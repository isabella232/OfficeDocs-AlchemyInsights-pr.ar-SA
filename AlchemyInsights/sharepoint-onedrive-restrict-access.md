---
title: تقييد الوصول في SharePoint أو OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700442"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="d8d09-102">تقييد الوصول في SharePoint أو OneDrive</span><span class="sxs-lookup"><span data-stu-id="d8d09-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="d8d09-103">هناك العديد من الطرق لتقييد الوصول إلى خدمات SharePoint Online/OneDrive.</span><span class="sxs-lookup"><span data-stu-id="d8d09-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="d8d09-104">يتم توضيح طرق تقييد الوصول المختلفة أدناه.</span><span class="sxs-lookup"><span data-stu-id="d8d09-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="d8d09-105">**قيد الأذونات**</span><span class="sxs-lookup"><span data-stu-id="d8d09-105">**Permission Restriction**</span></span>

<span data-ttu-id="d8d09-106">في SharePoint Online و OneDrive for Business ، قم بتقييد الوصول إلى عناصر مثل المواقع والملفات والمجلدات بمنح حق الوصول إلى هذه المجموعات/الأشخاص الذين يجب ان يملكون حق الوصول.</span><span class="sxs-lookup"><span data-stu-id="d8d09-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="d8d09-107">تخصيص الأذونات لقائمه أو مكتبه SharePoint</span><span class="sxs-lookup"><span data-stu-id="d8d09-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="d8d09-108">تخصيص أذونات موقع SharePoint</span><span class="sxs-lookup"><span data-stu-id="d8d09-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="d8d09-109">تغيير الأذونات علي مجلد فرعي</span><span class="sxs-lookup"><span data-stu-id="d8d09-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="d8d09-110">التحكم في الوصول من الاجهزه غير المدارة</span><span class="sxs-lookup"><span data-stu-id="d8d09-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="d8d09-111">بصفتك مسؤولا عموميا أو SharePoint ، يمكنك حظر الوصول إلى المحتوي SharePoint و OneDrive من الاجهزه غير المدارة أو تقييده (غير المرتبطة بالإعلانات المختلطة أو المتوافقة معها في Intune).</span><span class="sxs-lookup"><span data-stu-id="d8d09-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="d8d09-112">**تقييد موقع الشبكة**</span><span class="sxs-lookup"><span data-stu-id="d8d09-112">**Network Location Restriction**</span></span>

<span data-ttu-id="d8d09-113">بصفتك مسؤولا ، يمكنك التحكم في الوصول إلى موارد SharePoint و OneDrive استنادا إلى مواقع الشبكة المعرفة التي تثق بها.</span><span class="sxs-lookup"><span data-stu-id="d8d09-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="d8d09-114">يعرف هذا أيضا باسم النهج المستند إلى الموقع.</span><span class="sxs-lookup"><span data-stu-id="d8d09-114">This is also known as location-based policy.</span></span> <span data-ttu-id="d8d09-115">لمزيد من المعلومات ، يرجى مراجعه [التحكم في الوصول إلى بيانات SharePoint Online و OneDrive استنادا إلى موقع الشبكة](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="d8d09-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="d8d09-116">**قيد تامين الموقع**</span><span class="sxs-lookup"><span data-stu-id="d8d09-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="d8d09-117">في SharePoint Online ، تتوفر لديك القدرة علي تامين مجموعه مواقع مشتركه ، لذلك لا يوجد لدي اي شخص حق الوصول.</span><span class="sxs-lookup"><span data-stu-id="d8d09-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="d8d09-118">يتم تعيين ذلك عبر PowerShell و [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) باستخدام الخاصية [set سبوسيتي](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -لوكستاتي.</span><span class="sxs-lookup"><span data-stu-id="d8d09-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="d8d09-119">**منع المستخدمين من إنشاء مواقع أو مواقع فرعيه**</span><span class="sxs-lookup"><span data-stu-id="d8d09-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="d8d09-120">بصفتك مسؤول SharePoint أو مسؤول عمومي ، يمكنك السماح للمستخدمين بإنشاء مواقع SharePoint الخاصة بهم وأدارتها ، وتحديد نوع المواقع التي يمكنهم إنشاؤها ، وتحديد موقع المواقع.</span><span class="sxs-lookup"><span data-stu-id="d8d09-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="d8d09-121">لمزيد من المعلومات ، يرجى مراجعه [إنشاء موقع الاداره في SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="d8d09-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

