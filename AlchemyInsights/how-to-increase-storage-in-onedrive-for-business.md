---
title: كيفيه زيادة مساحة التخزين في OneDrive for Business
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ceaa6256-a9d9-4fef-a274-d7219365e07f
ms.openlocfilehash: 676b17d47ee5071ed45e8d6022eaa82b51fc4d51
ms.sourcegitcommit: ad2d185aa9e08c27c4a1c4803b679cc4e6305703
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/16/2020
ms.locfileid: "48488986"
---
# <a name="how-to-increase-storage-in-onedrive-for-business"></a><span data-ttu-id="9dde8-102">كيفيه زيادة مساحة التخزين في OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="9dde8-102">How to increase storage in OneDrive for Business</span></span>

<span data-ttu-id="9dde8-103">لتغيير التخزين الافتراضي لمستخدمي OneDrive الجدد والموجودين:</span><span class="sxs-lookup"><span data-stu-id="9dde8-103">To change the default storage for new and existing OneDrive users:</span></span>
  
- <span data-ttu-id="9dde8-104">انتقل إلى [صفحه التخزين في مركز أداره OneDrive](https://admin.onedrive.com/?v=StorageSettings)، وادخل مقدارا جديدا في GB ، ثم حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="9dde8-104">Go to the [Storage page of the OneDrive admin center](https://admin.onedrive.com/?v=StorageSettings), enter a new amount in GB, then select **Save**.</span></span>

<span data-ttu-id="9dde8-105">يتم تطبيق اعداد مساحة التخزين هذه علي كل المستخدمين الذين لم تعين حدود التخزين المحددة لهم.</span><span class="sxs-lookup"><span data-stu-id="9dde8-105">This storage space setting applies to all users for whom you haven't set specific storage limits.</span></span> <span data-ttu-id="9dde8-106">لتغيير مساحة التخزين لمستخدمين محددين ، استخدم Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9dde8-106">To change the storage space for specific users, use Microsoft PowerShell.</span></span> <span data-ttu-id="9dde8-107">للحصول علي معلومات حول كيفيه القيام بذلك ، راجع [تغيير مساحة التخزين الخاصة بالمستخدمين في OneDrive باستخدام PowerShell](https://docs.microsoft.com/onedrive/change-user-storage).</span><span class="sxs-lookup"><span data-stu-id="9dde8-107">For info on how to do this, see [Change your users' OneDrive storage space using PowerShell](https://docs.microsoft.com/onedrive/change-user-storage).</span></span>

<span data-ttu-id="9dde8-108">**ملاحظه**: يبدو انك ليس لديك خطه تتضمن مساحة تخزين غير محدوده.</span><span class="sxs-lookup"><span data-stu-id="9dde8-108">**NOTE**: It looks like you don't have a plan that includes unlimited storage.</span></span> <span data-ttu-id="9dde8-109">للحصول علي معلومات حول مساحة التخزين التي تاتي مع كل خطه ، راجع [وصف خدمه OneDrive For business](https://docs.microsoft.com/office365/servicedescriptions/onedrive-for-business-service-description).</span><span class="sxs-lookup"><span data-stu-id="9dde8-109">For info about the storage that comes with each plan, see [OneDrive for Business service description](https://docs.microsoft.com/office365/servicedescriptions/onedrive-for-business-service-description).</span></span>
  
<span data-ttu-id="9dde8-110">لزيادة مساحة التخزين في OneDrive for Business ، اختر اشتراكا يتضمن Onedrive for business **الخطة 2** أو **Office 365 E3**.</span><span class="sxs-lookup"><span data-stu-id="9dde8-110">To increase your storage in OneDrive for Business, choose a subscription that includes either **OneDrive for Business Plan 2** or **Office 365 E3**.</span></span>
  
<span data-ttu-id="9dde8-111">لتغيير الخطط ، في مركز الاداره ، انتقل إلى صفحه **فوتره** \> [المنتجات](https://go.microsoft.com/fwlink/p/?linkid=842054) ، وحدد الاشتراك الذي تريد تغييره ، ثم اختر **عرض الترقيات الموصي بها لمؤسسك**.</span><span class="sxs-lookup"><span data-stu-id="9dde8-111">To change plans, in the admin center, go to the **Billing** \> [Your products](https://go.microsoft.com/fwlink/p/?linkid=842054) page, select the subscription to change, then choose **View upgrades recommended for your org**.</span></span>
  
<span data-ttu-id="9dde8-112">للحصول علي مزيد من المعلومات حول تغيير الخطط و OneDrive for Business ، راجع [الترقية إلى خطه مختلفه](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan) [ووصف خدمه onedrive for business](https://docs.microsoft.com/office365/servicedescriptions/onedrive-for-business-service-description).</span><span class="sxs-lookup"><span data-stu-id="9dde8-112">For more information on changing plans and OneDrive for Business storage, see [Upgrade to a different plan](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan) and the [OneDrive for Business Service Description](https://docs.microsoft.com/office365/servicedescriptions/onedrive-for-business-service-description).</span></span>