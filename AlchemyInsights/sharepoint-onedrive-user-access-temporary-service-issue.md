---
title: مشكلات الأداء-SharePoint أو OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 2dc0cd5f1641298853443d364eb9434ec1d9cd5a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511135"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="8cc59-102">SharePoint أو OneDrive بطيئة أو غير قابلة للوصول أو غير متوفرة للعديد من المستخدمين</span><span class="sxs-lookup"><span data-stu-id="8cc59-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="8cc59-103">إذا كان موقع OneDrive أو SharePoint غير متوفر للعديد من المستخدمين الذين سبق لهم الوصول، فقد تكون هناك مشكلة في الخدمة المؤقتة.</span><span class="sxs-lookup"><span data-stu-id="8cc59-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="8cc59-104">[تحقق من لوحة معلومات صحة الخدمة](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="8cc59-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="8cc59-105">**إضافة المستخدم وترخيصه**</span><span class="sxs-lookup"><span data-stu-id="8cc59-105">**Add and license the user**</span></span>

<span data-ttu-id="8cc59-106">تأكد من [تعيين تراخيص للمستخدمين في Microsoft 365 للأعمال](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="8cc59-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="8cc59-107">**تعيين الأذونات**</span><span class="sxs-lookup"><span data-stu-id="8cc59-107">**Assign Permissions**</span></span>

<span data-ttu-id="8cc59-108">إذا تم تعيين ترخيص Sharepoint للمستخدم ولا يزال يتلقى رسالة رفض الوصول، فيرجى التأكد من أن لديهم [مستوى الإذن المناسب](https://docs.microsoft.com/sharepoint/understanding-permission-levels) الذي تم تعيينه.</span><span class="sxs-lookup"><span data-stu-id="8cc59-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="8cc59-109">**فكر في استخدام ميزة طلب الوصول**</span><span class="sxs-lookup"><span data-stu-id="8cc59-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="8cc59-110">تسمح [ميزة طلب الوصول](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) للأشخاص بطلب الوصول إلى المحتوى الذي ليس لديهم إذن برؤيته حاليًا.</span><span class="sxs-lookup"><span data-stu-id="8cc59-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="8cc59-111">**قد يؤدي السماح بالبرنامج النصي المخصص إلى رفض الوصول إلى المشكلات**</span><span class="sxs-lookup"><span data-stu-id="8cc59-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="8cc59-112">هناك بعض السيناريوهات حيث ميزة *السماح برنامج نصي مخصص* قد يكون تقديم الوصول رفض.</span><span class="sxs-lookup"><span data-stu-id="8cc59-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="8cc59-113">للحصول على قائمة بالميزات المتأثرة، اعتبارات الأمان والقدرة على تعطيل الميزة.</span><span class="sxs-lookup"><span data-stu-id="8cc59-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="8cc59-114">الرجاء زيارة [السماح أو منع البرنامج النصي المخصص.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span><span class="sxs-lookup"><span data-stu-id="8cc59-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

