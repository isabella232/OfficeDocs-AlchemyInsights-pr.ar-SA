---
title: استكشاف أخطاء الوصول مرفوض رسائل إلى أندريف لمواقع العمل
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 39f9b9b1ca22f6e5959e2b431fb373b0002c0a92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507798"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="e03fb-102">استكشاف أخطاء الوصول مرفوض رسائل إلى أندريف لمواقع العمل</span><span class="sxs-lookup"><span data-stu-id="e03fb-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="e03fb-103">تحدث هذه المشكلة غالباً عندما يكون مستخدم حذف وإعادة إنشاء بواسطة نفس اسم المستخدم الأساسي (UPN).</span><span class="sxs-lookup"><span data-stu-id="e03fb-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="e03fb-104">يتم إنشاء حساب جديد باستخدام قيمة PUID (المعرف الفريد ل Passport) مختلفة.</span><span class="sxs-lookup"><span data-stu-id="e03fb-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="e03fb-105">عندما يحاول المستخدم الوصول إلى مجموعة موقع أو أندريف بها، لدى المستخدم PUID غير صحيحة.</span><span class="sxs-lookup"><span data-stu-id="e03fb-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="e03fb-106">سيناريو ثاني يتضمن الدليل المزامنة مع وحدة "خدمة active Directory" تنظيمية (OU).</span><span class="sxs-lookup"><span data-stu-id="e03fb-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="e03fb-107">إذا كان المستخدمون قد مسبقاً بتسجيل الدخول إلى SharePoint، ثم يتم نقلها إلى OU مختلفة و resynced مع SharePoint، قد تواجه هذه المشكلة.</span><span class="sxs-lookup"><span data-stu-id="e03fb-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="e03fb-108">لحل هذه المشكلة يجب عليك استعادة UPN الأصلي باستخدام الخطوات المذكورة في المقالة،[استعادة مستخدم في Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="e03fb-108">To resolve this issue you should restore the original UPN with the steps in the article,[Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="e03fb-109">لا يمكنك استعادة المستخدم الأصلي يجب عليك إزالة الملف من الموقع أندريف باستخدام هذه الخطوات، [إزالة مستخدم من قائمة معلومات المستخدمين]().</span><span class="sxs-lookup"><span data-stu-id="e03fb-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="e03fb-110">بعد القيام بذلك، يمكنك التحقق من المستخدم لديه حقوق المسؤول إلى الموقع أندريف باتباع الخطوات التالية [إضافة المسؤول الخاص أندريف المستخدم](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="e03fb-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="e03fb-111">لمزيد من المعلومات حول مستويات الأذونات، راجع المقال، [فهم "مستويات الإذن" في SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="e03fb-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
