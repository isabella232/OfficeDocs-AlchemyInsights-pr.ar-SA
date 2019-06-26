---
title: استكشاف أخطاء الوصول مرفوض رسائل إلى أندريف لمواقع العمل
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: b394cc1441187133d8829cfc5fb0c1edbd71fd96
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223411"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="b9688-102">استكشاف أخطاء الوصول مرفوض رسائل إلى أندريف لمواقع العمل</span><span class="sxs-lookup"><span data-stu-id="b9688-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="b9688-103">تحدث هذه المشكلة غالباً عندما يكون مستخدم حذف وإعادة إنشاء بواسطة نفس اسم المستخدم الأساسي (UPN).</span><span class="sxs-lookup"><span data-stu-id="b9688-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="b9688-104">يتم إنشاء حساب جديد باستخدام قيمة PUID (المعرف الفريد ل Passport) مختلفة.</span><span class="sxs-lookup"><span data-stu-id="b9688-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="b9688-105">عندما يحاول المستخدم الوصول إلى مجموعة موقع أو أونيدريفي بها، لدى المستخدم PUID غير صحيحة.</span><span class="sxs-lookup"><span data-stu-id="b9688-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="b9688-106">سيناريو ثاني يتضمن الدليل المزامنة مع وحدة "خدمة active Directory" تنظيمية (OU).</span><span class="sxs-lookup"><span data-stu-id="b9688-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="b9688-107">إذا كان المستخدمون قد مسبقاً بتسجيل الدخول إلى SharePoint، ثم يتم نقلها إلى OU مختلفة و resynced مع SharePoint، قد تواجه هذه المشكلة.</span><span class="sxs-lookup"><span data-stu-id="b9688-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="b9688-108">لحل هذه المشكلة يجب عليك استعادة UPN الأصلي باستخدام الخطوات المذكورة في المقالة،[استعادة مستخدم في Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="b9688-108">To resolve this issue you should restore the original UPN with the steps in the article,[Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="b9688-109">بعد القيام بذلك، يمكنك التحقق من المستخدم لديه حقوق المسؤول إلى الموقع أندريف باتباع الخطوات التالية [إضافة المسؤول الخاص أندريف المستخدم](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="b9688-109">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="b9688-110">لمزيد من المعلومات حول مستويات الأذونات، راجع المقال، [فهم "مستويات الإذن" في SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="b9688-110">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
