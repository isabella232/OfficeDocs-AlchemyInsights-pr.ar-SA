---
title: حديث الموقع الجذر
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057663"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="f1ba6-102">موقع الحديثة كالموقع الجذر</span><span class="sxs-lookup"><span data-stu-id="f1ba6-102">Modern site as root site</span></span>

<span data-ttu-id="f1ba6-103">تمكين العملاء [الإصدار الهدف](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) الآن تجربة موقع الاتصالات الحديثة في الموقع الجذر الكلاسيكية للمستأجر SharePoint الخاصة بهم.</span><span class="sxs-lookup"><span data-stu-id="f1ba6-103">[Target Release](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) customers can now enable the modern communication site experience at the classic root site of their SharePoint tenant.</span></span>

<span data-ttu-id="f1ba6-104">يمكن تنشيط هذه الميزة عن طريق تشغيل cmdlet PowerShell بسيطة.</span><span class="sxs-lookup"><span data-stu-id="f1ba6-104">This feature can be activated by running a simple PowerShell cmdlet.</span></span> <span data-ttu-id="f1ba6-105">على نجاح تنفيذ أوامر PowerShell، سيكون الموقع الجذر لصفحة رئيسية موقع اتصال.</span><span class="sxs-lookup"><span data-stu-id="f1ba6-105">On the successful execution of the PowerShell command(s), the root site will have a new communication site home page.</span></span> <span data-ttu-id="f1ba6-106">تتوفر التفاصيل حول متطلبات PowerShell cmdlet وميزة في المقال [تمكين سبوكومسيتي](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="f1ba6-106">Details about the PowerShell cmdlet and feature requirements are available in the article [Enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span></span> 

<span data-ttu-id="f1ba6-107">أننا سوف تدريجيا المتداول هذا، إيقاف تشغيل بشكل افتراضي، للعملاء "الإصدار المستهدف" في أوائل مايو 2019، وطرح ستكون متاحة في جميع أنحاء العالم بنهاية يونيو عام 2019.</span><span class="sxs-lookup"><span data-stu-id="f1ba6-107">We'll be gradually rolling this out, off by default, to Targeted Release customers in early May 2019, and the roll out will be available worldwide by the end of June 2019.</span></span> <span data-ttu-id="f1ba6-108">متابعة للإشارة إلى [مركز](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) لميزات جديدة بحديث.</span><span class="sxs-lookup"><span data-stu-id="f1ba6-108">Continue to refer to the [Message Center](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) for other new features with Modern.</span></span> 

<span data-ttu-id="f1ba6-109">**هام**: لا تقم بحذف الموقع الجذر الكلاسيكية لإنشاء "موقع الاتصالات" الحديثة.</span><span class="sxs-lookup"><span data-stu-id="f1ba6-109">**Important**: Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="f1ba6-110">وهذا غير معتمد من قبل Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f1ba6-110">This is not supported by Microsoft.</span></span> <span data-ttu-id="f1ba6-111">حذف الموقع الجذر سيجعل كافة مواقع SharePoint في المؤسسة الخاصة بك غير متاحة لكافة المستخدمين، حتى يمكنك استعادة الموقع أو إنشاء موقع جديد على نفس العنوان.</span><span class="sxs-lookup"><span data-stu-id="f1ba6-111">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> 
 
 