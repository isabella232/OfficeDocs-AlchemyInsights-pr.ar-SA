---
title: استكشاف أخطاء الوصول وإصلاحها رفض الرسائل إلى اندريف لمواقع العمل
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9d8aba4e53a1e0505a430296bb1c11713ea2ce7b
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051592"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="6e225-102">استكشاف أخطاء الوصول وإصلاحها رفض الرسائل إلى اندريف لمواقع العمل</span><span class="sxs-lookup"><span data-stu-id="6e225-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="6e225-103">تحدث هذه المشكلة بشكل متكرر عند حذف مستخدم وأعاده إنشائه بنفس الاسم الأساسي للمستخدم (UPN).</span><span class="sxs-lookup"><span data-stu-id="6e225-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="6e225-104">يتم إنشاء الحساب الجديد باستخدام قيمه PUID (معرف فريد لPassport) مختلفه.</span><span class="sxs-lookup"><span data-stu-id="6e225-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="6e225-105">عندما يحاول المستخدم الوصول إلى مجموعه موقع أو اندريف الخاصة بهم ، المستخدم لديه PUID غير صحيحه.</span><span class="sxs-lookup"><span data-stu-id="6e225-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="6e225-106">يتضمن السيناريو الثاني مزامنة الدليل مع الوحدة التنظيمية "Active Directory" (OU).</span><span class="sxs-lookup"><span data-stu-id="6e225-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="6e225-107">إذا كان المستخدمون بالفعل تسجيل الدخول إلى SharePoint ، ومن ثم يتم نقلها إلى OU مختلفه resynced مع SharePoint ، فانها قد تواجه هذه المشكلة.</span><span class="sxs-lookup"><span data-stu-id="6e225-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="6e225-108">لحل هذه المشكلة يجب استعاده UPN الأصلي مع الخطوات التالية في المقالة ، [استعاده مستخدم في Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="6e225-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="6e225-109">إذا كان لا يمكنك استعاده المستخدم الأصلي يجب أزاله المستخدم القديم من موقع اندريف باستخدام هذه الخطوات [أزاله مستخدم من قائمه معلومات المستخدم]().</span><span class="sxs-lookup"><span data-stu-id="6e225-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="6e225-110">بعد الانتهاء من ذلك ، يمكنك التحقق من ان المستخدم لديه حقوق المسؤول إلى موقع اندريف باتباع الخطوات التالية [لأضافه المسؤول لاندريف المستخدم](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="6e225-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="6e225-111">لمزيد من المعلومات حول مستويات الأذونات ، راجع المقالة ، [فهم مستويات الأذونات في SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="6e225-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
