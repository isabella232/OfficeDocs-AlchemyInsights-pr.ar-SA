---
title: مشاكل الأداء SharePoint أو أندريف
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 3b04e811b69a1f9d652abbd603c3c09df068480c
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719504"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="cd11b-102">SharePoint أو أندريف بطيئة، غير قابلة للوصول أو غير متاحة للعديد من المستخدمين</span><span class="sxs-lookup"><span data-stu-id="cd11b-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="cd11b-103">في حالة عدم توفر للعديد من المستخدمين الذين تم الوصول إلى موقع SharePoint أو أندريف، قد يكون هناك مشكلة في خدمة مؤقت.</span><span class="sxs-lookup"><span data-stu-id="cd11b-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="cd11b-104">[تحقق من لوحة المعلومات الصحية الخدمة](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="cd11b-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

## <a name="add-and-license-the-user"></a><span data-ttu-id="cd11b-105">إضافة وترخيص المستخدم</span><span class="sxs-lookup"><span data-stu-id="cd11b-105">Add and license the user</span></span>

<span data-ttu-id="cd11b-106">تأكد من ذلك يمكنك [تعيين التراخيص للمستخدمين في Office 365 للعمل](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="cd11b-106">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>


## <a name="assign-permissions"></a><span data-ttu-id="cd11b-107">تعيين أذونات</span><span class="sxs-lookup"><span data-stu-id="cd11b-107">Assign Permissions</span></span>

<span data-ttu-id="cd11b-108">إذا تم تعيين ترخيص Sharepoint المستخدم ويزال يتلقى رسالة رفض وصول، الرجاء التأكد من لديهم [مستوى الأذونات المناسبة](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) المعينة.</span><span class="sxs-lookup"><span data-stu-id="cd11b-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) assigned.</span></span>

## <a name="consider-using-the-access-request-feature"></a><span data-ttu-id="cd11b-109">يمكنك استخدام ميزة طلب الوصول</span><span class="sxs-lookup"><span data-stu-id="cd11b-109">Consider using the access request feature</span></span>

<span data-ttu-id="cd11b-110">تسمح [ميزة طلب الوصول](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) الأشخاص لطلب الوصول إلى محتوى ليس حاليا لديهم إذن بعرضها.</span><span class="sxs-lookup"><span data-stu-id="cd11b-110">The [access request feature](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

## <a name="allow-custom-script-may-cause-access-denied-issues"></a><span data-ttu-id="cd11b-111">السماح بالبرامج النصية المخصصة قد يسبب مشاكل تم رفض الوصول</span><span class="sxs-lookup"><span data-stu-id="cd11b-111">Allow custom script may cause access denied issues</span></span>

<span data-ttu-id="cd11b-112">هناك بعض السيناريوهات حيث ميزة *السماح بالبرنامج النصي المخصص* قد يكون تقديم رفض وصول.</span><span class="sxs-lookup"><span data-stu-id="cd11b-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="cd11b-113">لقائمة الميزات المتأثرة واعتبارات الأمان وإمكانية تعطيل الميزة.</span><span class="sxs-lookup"><span data-stu-id="cd11b-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="cd11b-114">الرجاء زيارة [السماح أو منع البرامج النصية المخصصة](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="cd11b-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span></span>

