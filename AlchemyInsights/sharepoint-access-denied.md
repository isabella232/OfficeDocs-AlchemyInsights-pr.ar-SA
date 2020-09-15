---
title: استكشاف أخطاء الوصول إلى الرسائل التي تم رفضها
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: f49cfc50142b3d98a5f431a38e9a943eb5624523
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691670"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="8c6e6-102">استكشاف أخطاء الوصول إلى الرسائل التي تم رفضها</span><span class="sxs-lookup"><span data-stu-id="8c6e6-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="8c6e6-103">إذا تلقيت رسالة تفيد بأنه تم رفض الوصول عند محاولة استعراض موقع Sharepoint Online ، فالرجاء مراجعه المقالات التالية.</span><span class="sxs-lookup"><span data-stu-id="8c6e6-103">If you are receiving an access denied message when attempting to browse a Sharepoint Online site, please see the below articles.</span></span>

<span data-ttu-id="8c6e6-104">**أضافه المستخدم وترخيصه**</span><span class="sxs-lookup"><span data-stu-id="8c6e6-104">**Add and License the user**</span></span>

<span data-ttu-id="8c6e6-105">تاكد من [تعيين تراخيص للمستخدمين في Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="8c6e6-105">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>

<span data-ttu-id="8c6e6-106">**تعيين الأذونات**</span><span class="sxs-lookup"><span data-stu-id="8c6e6-106">**Assign Permissions**</span></span>

<span data-ttu-id="8c6e6-107">إذا تم تعيين ترخيص Sharepoint إلى المستخدم وكان لا يزال يتلقى رسالة برفض الوصول ، فالرجاء التاكد من انه تم [تعيين مستوي الأذونات المناسب](https://docs.microsoft.com/sharepoint/understanding-permission-levels)لها.</span><span class="sxs-lookup"><span data-stu-id="8c6e6-107">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level assigned](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>

<span data-ttu-id="8c6e6-108">**خذ في الاعتبار استخدام ميزه طلبات الوصول**</span><span class="sxs-lookup"><span data-stu-id="8c6e6-108">**Consider using the access request feature**</span></span>

<span data-ttu-id="8c6e6-109">تسمح ميزه [طلبات access](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) للأشخاص بطلب الوصول إلى المحتوي الذي لا يملكون الاذن بالاطلاع عليه حاليا.</span><span class="sxs-lookup"><span data-stu-id="8c6e6-109">The [access request](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) feature allows people to request access to content that they do not currently have permission to see.</span></span> 

<span data-ttu-id="8c6e6-110">**قد يؤدي السماح بالبرنامج النصي المخصص إلى مشاكل رفض الوصول**</span><span class="sxs-lookup"><span data-stu-id="8c6e6-110">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="8c6e6-111">هناك بعض السيناريوهات التي قد يكون فيها الميزة "السماح ببرمجه نصيه مخصصه" من تقديم رفض الوصول.</span><span class="sxs-lookup"><span data-stu-id="8c6e6-111">There are certain scenarios where the "Allow custom script" feature may be presenting an access denied.</span></span> <span data-ttu-id="8c6e6-112">للحصول علي قائمه بالميزات المتاثره ، واعتبارات الأمان والقدرة علي تعطيل الميزة.</span><span class="sxs-lookup"><span data-stu-id="8c6e6-112">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="8c6e6-113">يرجى زيارة [برنامج نصي مخصص أو السماح به أو منعه](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span><span class="sxs-lookup"><span data-stu-id="8c6e6-113">Please visit , [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span></span>

<span data-ttu-id="8c6e6-114">ملاحظه: إذا لم يكن موقع OneDrive أو SharePoint متوفرا لعده مستخدمين لديهم حق الوصول ، فقد تكون هناك مشكله خدمه مؤقته.</span><span class="sxs-lookup"><span data-stu-id="8c6e6-114">Note: If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="8c6e6-115">[تحقق من لوحه معلومات حماية الخدمة](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="8c6e6-115">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


  

