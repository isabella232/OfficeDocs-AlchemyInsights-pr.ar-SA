---
title: مشكلات الأداء-SharePoint أو اندريف
ms.author: pebaum
author: pebaum
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 2db0a9442b9fdf1752b654f7c188e641e0a274cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053788"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="eb235-102">SharePoint أو اندريف بطيئه أو غير قابله للوصول أو غير متوفرة لمستخدمين متعددين</span><span class="sxs-lookup"><span data-stu-id="eb235-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="eb235-103">إذا كان موقع اندريف أو SharePoint غير متوفر للعديد من المستخدمين الذين كان لديهم حق الوصول مسبقا ، قد تكون هناك مشكله خدمه مؤقته.</span><span class="sxs-lookup"><span data-stu-id="eb235-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="eb235-104">[تحقق من لوحه معلومات صحة الخدمة](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="eb235-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="eb235-105">**أضافه المستخدم وترخيصه**</span><span class="sxs-lookup"><span data-stu-id="eb235-105">**Add and license the user**</span></span>

<span data-ttu-id="eb235-106">تاكد من [تعيين التراخيص للمستخدمين في Office 365 للعمل](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="eb235-106">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>


<span data-ttu-id="eb235-107">**تعيين الأذونات**</span><span class="sxs-lookup"><span data-stu-id="eb235-107">**Assign Permissions**</span></span>

<span data-ttu-id="eb235-108">إذا تم تعيين ترخيص Sharepoint للمستخدم ولا يزال يتلقى رسالة تم رفض الوصول اليها ، الرجاء التاكد من ان لديهم [مستوي الاذن المناسب](https://docs.microsoft.com/sharepoint/understanding-permission-levels) المعين.</span><span class="sxs-lookup"><span data-stu-id="eb235-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="eb235-109">**النظر في استخدام ميزه طلب الوصول**</span><span class="sxs-lookup"><span data-stu-id="eb235-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="eb235-110">تسمح [ميزه طلب الوصول](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) للأشخاص بطلب الوصول إلى المحتوي الذي ليس لديهم حاليا اذن لرؤيته.</span><span class="sxs-lookup"><span data-stu-id="eb235-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="eb235-111">**السماح لبرنامج نصي مخصص قد يؤدي إلى رفض الوصول المشكلات**</span><span class="sxs-lookup"><span data-stu-id="eb235-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="eb235-112">هناك بعض وحدات السيناريو حيث *السماح ميزه البرنامج النصي المخصص* قد يتم تقديم رفض وصول.</span><span class="sxs-lookup"><span data-stu-id="eb235-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="eb235-113">للحصول علي قائمه بالميزات المتاثره ، اعتبارات الأمان والقدرة علي تعطيل الميزة.</span><span class="sxs-lookup"><span data-stu-id="eb235-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="eb235-114">يرجى زيارة [السماح أو منع البرنامج النصي المخصص](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="eb235-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

