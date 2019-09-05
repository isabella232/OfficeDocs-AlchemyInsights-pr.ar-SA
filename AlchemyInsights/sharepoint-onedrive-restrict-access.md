---
title: تقييد الوصول في SharePoint أو أندريف
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750651"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="521c2-102">تقييد الوصول في SharePoint أو أندريف</span><span class="sxs-lookup"><span data-stu-id="521c2-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="521c2-103">هناك العديد من الطرق لتقييد الوصول إلى خدمات SharePoint على الإنترنت/أندريف.</span><span class="sxs-lookup"><span data-stu-id="521c2-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="521c2-104">وترد أدناه أساليب تقييد الوصول المختلفة هذه.</span><span class="sxs-lookup"><span data-stu-id="521c2-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="521c2-105">**تقييد الإذن**</span><span class="sxs-lookup"><span data-stu-id="521c2-105">**Permission Restriction**</span></span>

<span data-ttu-id="521c2-106">في SharePoint Online وOneDrive for Business، نقوم بتقييد الوصول إلى عناصر مثل المواقع والملفات والمجلدات من خلال منح حق الوصول فقط إلى تلك المجموعات/الأفراد الذين يجب أن يكون لديهم حق الوصول.</span><span class="sxs-lookup"><span data-stu-id="521c2-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="521c2-107">تخصيص الأذونات لقائمة أو مكتبة SharePoint</span><span class="sxs-lookup"><span data-stu-id="521c2-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="521c2-108">تخصيص أذونات موقع SharePoint</span><span class="sxs-lookup"><span data-stu-id="521c2-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="521c2-109">تغيير الأذونات على مجلد فرعي</span><span class="sxs-lookup"><span data-stu-id="521c2-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="521c2-110">التحكم في الوصول من الأجهزة غير المُدارة</span><span class="sxs-lookup"><span data-stu-id="521c2-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="521c2-111">كمسؤول SharePoint أو عمومي في Office 365، يمكنك حظر أو تقييد الوصول إلى محتوى SharePoint و OneDrive من الأجهزة غير المُدارة (تلك التي لم يتم ضمها AD المختلطأو متوافقة في إينتوني).</span><span class="sxs-lookup"><span data-stu-id="521c2-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="521c2-112">**تقييد موقع الشبكة**</span><span class="sxs-lookup"><span data-stu-id="521c2-112">**Network Location Restriction**</span></span>

<span data-ttu-id="521c2-113">بصفتك مسؤول تكنولوجيا المعلومات، يمكنك التحكم في الوصول إلى موارد SharePoint وOneDrive استنادًا إلى مواقع شبكة الاتصال المحددة التي تثق بها.</span><span class="sxs-lookup"><span data-stu-id="521c2-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="521c2-114">يُعرف هذا أيضًا بالسياسة المستندة إلى الموقع.</span><span class="sxs-lookup"><span data-stu-id="521c2-114">This is also known as location-based policy.</span></span> <span data-ttu-id="521c2-115">لمزيد من المعلومات، الرجاء [مراجعة التحكم في الوصول إلى بيانات SharePoint عبر الإنترنت وOneDrive استناداً إلى موقع الشبكة](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="521c2-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="521c2-116">**تقييد تأمين الموقع**</span><span class="sxs-lookup"><span data-stu-id="521c2-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="521c2-117">داخل SharePoint على الإنترنت لديك القدرة على تأمين مجموعة موقع، لذلك لا أحد لديه حق الوصول.</span><span class="sxs-lookup"><span data-stu-id="521c2-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="521c2-118">يتم تعيين هذا عبر PowerShell و [Shell إدارة SharePoint عبر الإنترنت](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) باستخدام [الخاصية مجموعة SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) لوكستيت.</span><span class="sxs-lookup"><span data-stu-id="521c2-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="521c2-119">**تقييد المستخدمين من إنشاء مواقع أو مواقع فرعية**</span><span class="sxs-lookup"><span data-stu-id="521c2-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="521c2-120">بصفتك مسؤول SharePoint أو مسؤول عمومي Office 365، يمكنك السماح للمستخدمين بإنشاء وإدارة مواقع SharePoint الخاصة بهم، وتحديد نوع المواقع التي يمكنهم إنشاؤها، وتحديد موقع المواقع.</span><span class="sxs-lookup"><span data-stu-id="521c2-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="521c2-121">لمزيد من المعلومات، الرجاء [مراجعة إدارة إنشاء الموقع في SharePoint على الإنترنت](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="521c2-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

