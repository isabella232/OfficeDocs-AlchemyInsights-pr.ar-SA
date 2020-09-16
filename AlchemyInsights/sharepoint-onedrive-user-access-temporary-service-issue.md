---
title: مشاكل الأداء-SharePoint أو OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771231"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="ad8c3-102">SharePoint أو OneDrive البطيء أو القابل للوصول أو غير المتاح لعده مستخدمين</span><span class="sxs-lookup"><span data-stu-id="ad8c3-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="ad8c3-103">إذا لم يكن موقع OneDrive أو SharePoint متوفرا لعده مستخدمين لديهم حق الوصول ، فقد تكون هناك مشكله خدمه مؤقته.</span><span class="sxs-lookup"><span data-stu-id="ad8c3-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="ad8c3-104">[تحقق من لوحه معلومات حماية الخدمة](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="ad8c3-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="ad8c3-105">**أضافه المستخدم وترخيصه**</span><span class="sxs-lookup"><span data-stu-id="ad8c3-105">**Add and license the user**</span></span>

<span data-ttu-id="ad8c3-106">تاكد من [تعيين تراخيص للمستخدمين في Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="ad8c3-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="ad8c3-107">**تعيين الأذونات**</span><span class="sxs-lookup"><span data-stu-id="ad8c3-107">**Assign Permissions**</span></span>

<span data-ttu-id="ad8c3-108">إذا تم تعيين ترخيص Sharepoint إلى المستخدم وكان لا يزال يتلقى رسالة برفض الوصول ، فالرجاء التاكد من انه تم تعيين [مستوي الأذونات المناسب](https://docs.microsoft.com/sharepoint/understanding-permission-levels) لها.</span><span class="sxs-lookup"><span data-stu-id="ad8c3-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="ad8c3-109">**خذ في الاعتبار استخدام ميزه طلبات الوصول**</span><span class="sxs-lookup"><span data-stu-id="ad8c3-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="ad8c3-110">تسمح [ميزه طلبات access](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) للأشخاص بطلب الوصول إلى المحتوي الذي لا يملكون الاذن بالاطلاع عليه حاليا.</span><span class="sxs-lookup"><span data-stu-id="ad8c3-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="ad8c3-111">**قد يؤدي السماح بالبرنامج النصي المخصص إلى مشاكل رفض الوصول**</span><span class="sxs-lookup"><span data-stu-id="ad8c3-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="ad8c3-112">هناك بعض السيناريوهات التي قد يكون فيها *السماح لميزه البرامج النصية المخصصة* بتقديم رفض الوصول.</span><span class="sxs-lookup"><span data-stu-id="ad8c3-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="ad8c3-113">للحصول علي قائمه بالميزات المتاثره ، واعتبارات الأمان والقدرة علي تعطيل الميزة.</span><span class="sxs-lookup"><span data-stu-id="ad8c3-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="ad8c3-114">يرجى زيارة [السماح بالبرامج النصية المخصصة أو منعها](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="ad8c3-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

