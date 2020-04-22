---
title: استكشاف الأخطاء وإصلاحها الوصول رفض الرسائل إلى مواقع OneDrive للأعمال
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a83936acf969926c113b28ceb22b006cdb96e2b4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692788"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="798ff-102">استكشاف الأخطاء وإصلاحها الوصول رفض الرسائل إلى مواقع OneDrive للأعمال</span><span class="sxs-lookup"><span data-stu-id="798ff-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="798ff-103">تحدث هذه المشكلة بشكل متكرر عند حذف مستخدم وإعادة إنشائه بنفس اسم المستخدم الرئيسي (UPN).</span><span class="sxs-lookup"><span data-stu-id="798ff-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="798ff-104">يتم إنشاء الحساب الجديد باستخدام قيمة PUID مختلفة (معرف فريد من جواز السفر).</span><span class="sxs-lookup"><span data-stu-id="798ff-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="798ff-105">عندما يحاول المستخدم الوصول إلى مجموعة موقع أو OneDrive الخاص بهم، يكون لدى المستخدم PUID غير صحيح.</span><span class="sxs-lookup"><span data-stu-id="798ff-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="798ff-106">يتضمن سيناريو الثاني مزامنة الدليل مع وحدة تنظيمية "الدليل النشط" (OU).</span><span class="sxs-lookup"><span data-stu-id="798ff-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="798ff-107">إذا قام المستخدمون بتسجيل الدخول بالفعل إلى SharePoint، ثم تم نقلهم إلى OU مختلف وإعادة مزامنتهم مع SharePoint، فقد يواجهون هذه المشكلة.</span><span class="sxs-lookup"><span data-stu-id="798ff-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="798ff-108">لحل هذه المشكلة يجب استعادة UPN الأصلي مع الخطوات في المقالة استعادة [مستخدم في Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="798ff-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="798ff-109">إذا لم تتمكن من استعادة المستخدم الأصلي يجب إزالة المستخدم القديم من موقع OneDrive باستخدام هذه الخطوات، [قم بإزالة مستخدم من قائمة معلومات المستخدم]().</span><span class="sxs-lookup"><span data-stu-id="798ff-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="798ff-110">بعد الانتهاء من ذلك، يمكنك التحقق من أن المستخدم لديه حقوق المسؤول إلى موقع OneDrive باتباع الخطوات لإضافة [المسؤول لـ OneDrive للمستخدم](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span><span class="sxs-lookup"><span data-stu-id="798ff-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="798ff-111">لمزيد من المعلومات حول مستويات الأذونات، راجع المقالة، [فهم مستويات الأذونات في SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="798ff-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
