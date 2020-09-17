---
title: كيفيه زيادة مساحة التخزين في OneDrive for Business
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ceaa6256-a9d9-4fef-a274-d7219365e07f
ms.openlocfilehash: 53eabf6c87dead3b7309c7da1f8a590940127169
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780082"
---
# <a name="how-to-increase-storage-in-onedrive-for-business"></a><span data-ttu-id="91374-102">كيفيه زيادة مساحة التخزين في OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="91374-102">How to increase storage in OneDrive for Business</span></span>

<span data-ttu-id="91374-103">لتغيير التخزين الافتراضي لمستخدمي OneDrive الجدد والموجودين:</span><span class="sxs-lookup"><span data-stu-id="91374-103">To change the default storage for new and existing OneDrive users:</span></span>
  
- <span data-ttu-id="91374-104">انتقل إلى [صفحه التخزين في مركز أداره OneDrive](https://admin.onedrive.com/?v=StorageSettings)، ثم ادخل مبلغا جديدا بالغيغابايت.</span><span class="sxs-lookup"><span data-stu-id="91374-104">Go to the [Storage page of the OneDrive admin center](https://admin.onedrive.com/?v=StorageSettings), and then enter a new amount in GB.</span></span>

<span data-ttu-id="91374-105">يتم تطبيق اعداد مساحة التخزين هذه علي كل المستخدمين الذين لم تعين حدود التخزين المحددة لهم.</span><span class="sxs-lookup"><span data-stu-id="91374-105">This storage space setting applies to all users for whom you haven't set specific storage limits.</span></span> <span data-ttu-id="91374-106">لتغيير مساحة التخزين لمستخدمين محددين ، يجب استخدام Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="91374-106">To change the storage space for specific users, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="91374-107">للحصول علي معلومات حول كيفيه القيام بذلك ، راجع [تغيير مساحة التخزين الخاصة بالمستخدمين في OneDrive باستخدام PowerShell](https://go.microsoft.com/fwlink/?linkid=866402).</span><span class="sxs-lookup"><span data-stu-id="91374-107">For info on how to do this, see [Change your users' OneDrive storage space using PowerShell](https://go.microsoft.com/fwlink/?linkid=866402).</span></span>

<span data-ttu-id="91374-108">**ملاحظه**: يبدو انك ليس لديك خطه تتضمن مساحة تخزين غير محدوده.</span><span class="sxs-lookup"><span data-stu-id="91374-108">**NOTE**: It looks like you don't have a plan that includes unlimited storage.</span></span> <span data-ttu-id="91374-109">للحصول علي معلومات حول مساحة التخزين التي تاتي مع كل خطه ، راجع [وصف خدمه OneDrive For business](https://go.microsoft.com/fwlink/p/?LinkID=826071).</span><span class="sxs-lookup"><span data-stu-id="91374-109">For info about the storage that comes with each plan, see [OneDrive for Business service description](https://go.microsoft.com/fwlink/p/?LinkID=826071).</span></span>
  
<span data-ttu-id="91374-110">لزيادة مساحة التخزين في OneDrive for Business ، اختر اشتراكا يتضمن **onedrive** for Business أو **Office 365 Enterprise E3**.</span><span class="sxs-lookup"><span data-stu-id="91374-110">To increase your storage in OneDrive for Business, choose a subscription that includes either **OneDrive for Business Plan 2** or **Office 365 Enterprise E3**.</span></span> 
  
<span data-ttu-id="91374-111">لتغيير الخطط ، في مركز أداره Microsoft 365 ، انتقل إلى صفحه **الفوترة** \> **[الخاصة بالمنتجات](https://go.microsoft.com/fwlink/p/?linkid=842054)** ، وحدد الاشتراك الذي تريد تغييره ، ثم اختر علامة التبويب **ترقيه** .</span><span class="sxs-lookup"><span data-stu-id="91374-111">To change plans, in the Microsoft 365 admin center, go to the **Billing** \> **[Your products](https://go.microsoft.com/fwlink/p/?linkid=842054)** page, select the subscription to change, and then choose the **Upgrade** tab.</span></span>
  
<span data-ttu-id="91374-112">للحصول علي مزيد من المعلومات حول تبديل الخطط ومساحة التخزين في OneDrive for Business ، راجع [التبديل إلى خطه Microsoft 365 for business مختلفه](https://go.microsoft.com/fwlink/?LinkId=2031117) [ووصف خدمه OneDrive for business](https://go.microsoft.com/fwlink/p/?LinkId-2031122).</span><span class="sxs-lookup"><span data-stu-id="91374-112">For more information on switching plans and OneDrive for Business storage, see [Switch to a different Microsoft 365 for business plan](https://go.microsoft.com/fwlink/?LinkId=2031117) and the [OneDrive for Business Service Description](https://go.microsoft.com/fwlink/p/?LinkId-2031122).</span></span>