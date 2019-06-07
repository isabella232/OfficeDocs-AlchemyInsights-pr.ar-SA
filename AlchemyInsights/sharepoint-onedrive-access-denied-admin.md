---
title: استكشاف أخطاء رسائل "رفض الوصول"
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: c204f1889e03886fdfd3d1c760a4a2beb82b0836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760328"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="d64cf-102">استكشاف أخطاء رسائل "رفض الوصول" في "مركز مسؤول" Sharepoint/أونيدريفي</span><span class="sxs-lookup"><span data-stu-id="d64cf-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="d64cf-103">إذا كنت تتلقى رسالة وصول مرفوض عند محاولة الاستعراض إلى "مركز مسؤول" Sharepoint/أندريف، الرجاء التأكد من أن تقوم [تعيين ترخيص للمستخدم](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="d64cf-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="d64cf-104">إذا كان المستخدم لديه ترخيص، يجب أيضا التأكد من أنها [المعين لدور مسؤول](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) الوصول إليها مراكز الإدارة.</span><span class="sxs-lookup"><span data-stu-id="d64cf-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="d64cf-105">قد تحدث هذه المشكلة أيضا عند حذف مستخدم وإعادة إنشائها باستخدام نفس اسم المستخدم الأساسي (UPN).</span><span class="sxs-lookup"><span data-stu-id="d64cf-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="d64cf-106">يتم إنشاء حساب جديد باستخدام قيمة PUID (المعرف الفريد ل Passport) مختلفة.</span><span class="sxs-lookup"><span data-stu-id="d64cf-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="d64cf-107">عندما يحاول المستخدم الوصول إلى مجموعة موقع أو أندريف بها، لدى المستخدم PUID غير صحيحة.</span><span class="sxs-lookup"><span data-stu-id="d64cf-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="d64cf-108">سيناريو ثاني يتضمن الدليل المزامنة مع وحدة "خدمة active Directory" تنظيمية (OU).</span><span class="sxs-lookup"><span data-stu-id="d64cf-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="d64cf-109">إذا كان المستخدمون قد مسبقاً بتسجيل الدخول إلى SharePoint، ثم يتم نقلها إلى OU مختلفة و resynced مع SharePoint، قد تواجه هذه المشكلة.</span><span class="sxs-lookup"><span data-stu-id="d64cf-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="d64cf-110">لحل هذه المشكلة، يجب عليك استعادة UPN الأصلي باستخدام الخطوات المذكورة في المقالة، [استعادة مستخدم في Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="d64cf-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="d64cf-111">ملاحظة: إذا لم يتوفر أحد مراكز أندريف أو مسؤول SharePoint للعديد من المستخدمين الذين تم الوصول، قد يكون هناك مشكلة في خدمة مؤقت.</span><span class="sxs-lookup"><span data-stu-id="d64cf-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="d64cf-112">[تحقق من لوحة المعلومات الصحية الخدمة](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="d64cf-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


