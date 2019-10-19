---
title: تقييد الوصول في SharePoint أو اندريف
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750651"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="7c225-102">تقييد الوصول في SharePoint أو اندريف</span><span class="sxs-lookup"><span data-stu-id="7c225-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="7c225-103">هناك العديد من الطرق لتقييد الوصول إلى خدمات SharePoint علي الإنترنت/اندريف.</span><span class="sxs-lookup"><span data-stu-id="7c225-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="7c225-104">هذه الطرق المختلفة لتقييد الوصول موضحه أدناه.</span><span class="sxs-lookup"><span data-stu-id="7c225-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="7c225-105">**تقييد الأذونات**</span><span class="sxs-lookup"><span data-stu-id="7c225-105">**Permission Restriction**</span></span>

<span data-ttu-id="7c225-106">في SharePoint علي الإنترنت و اندريف للعمل ، ونحن تقييد الوصول إلى العناصر مثل المواقع والملفات والمجلدات عن طريق منح حق الوصول إلى تلك المجموعات/الافراد الذين يجب ان يكون الوصول.</span><span class="sxs-lookup"><span data-stu-id="7c225-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="7c225-107">تخصيص أذونات لقائمه أو مكتبه SharePoint</span><span class="sxs-lookup"><span data-stu-id="7c225-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="7c225-108">تخصيص أذونات موقع SharePoint</span><span class="sxs-lookup"><span data-stu-id="7c225-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="7c225-109">تغيير الأذونات علي مجلد فرعي</span><span class="sxs-lookup"><span data-stu-id="7c225-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="7c225-110">التحكم في الوصول من الاجهزه غير المدارة</span><span class="sxs-lookup"><span data-stu-id="7c225-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="7c225-111">كمسؤول SharePoint أو العمومية في Office 365 ، يمكنك حظر أو تقييد الوصول إلى محتوي SharePoint و OneDrive من الاجهزه غير المدارة (تلك غير المختلطة AD منضمة أو متوافقة في اينتوني).</span><span class="sxs-lookup"><span data-stu-id="7c225-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="7c225-112">**تقييد موقع الشبكة**</span><span class="sxs-lookup"><span data-stu-id="7c225-112">**Network Location Restriction**</span></span>

<span data-ttu-id="7c225-113">بصفتك مسؤول تكنولوجيا الاتصال ، يمكنك التحكم في الوصول إلى موارد SharePoint و OneDrive استنادا إلى مواقع الشبكة المعرفة التي تثق بها.</span><span class="sxs-lookup"><span data-stu-id="7c225-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="7c225-114">ويعرف هذا أيضا باسم النهج المستند إلى الموقع.</span><span class="sxs-lookup"><span data-stu-id="7c225-114">This is also known as location-based policy.</span></span> <span data-ttu-id="7c225-115">لمزيد من المعلومات ، الرجاء مراجعه [التحكم بالوصول إلى SharePoint علي الإنترنت والبيانات اندريف استنادا إلى موقع شبكه الاتصال](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="7c225-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="7c225-116">**تقييد قفل الموقع**</span><span class="sxs-lookup"><span data-stu-id="7c225-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="7c225-117">داخل SharePoint علي الإنترنت لديك القدرة علي تامين مجموعه موقع ، لذلك لا أحد لديه حق الوصول.</span><span class="sxs-lookup"><span data-stu-id="7c225-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="7c225-118">يتم تعيين هذا عبر PowerShell و [Shell أداره SharePoint علي الإنترنت](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) باستخدام الخاصية [مجموعه sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.</span><span class="sxs-lookup"><span data-stu-id="7c225-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="7c225-119">**تقييد المستخدمين من إنشاء مواقع أو مواقعه فرعيه**</span><span class="sxs-lookup"><span data-stu-id="7c225-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="7c225-120">كمسؤول SharePoint أو المسؤول العمومي Office 365 ، يمكنك السماح للمستخدمين إنشاء وأداره مواقع SharePoint الخاصة بهم ، وتحديد اي نوع من المواقع التي يمكن إنشاؤها ، وتحديد موقع المواقع.</span><span class="sxs-lookup"><span data-stu-id="7c225-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="7c225-121">لمزيد من المعلومات ، الرجاء مراجعه [أداره إنشاء الموقع في SharePoint علي الإنترنت](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="7c225-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

