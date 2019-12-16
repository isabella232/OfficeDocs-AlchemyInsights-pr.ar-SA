---
title: استكشاف أخطاء رسائل "رفض الوصول" وإصلاحها
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 57919e6dbd81a5bf3b17fb067485e8eec23b7d4c
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051412"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="567a7-102">استكشاف أخطاء رسائل "رفض الوصول" في مركز مسؤول Sharepoint/اندريف وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="567a7-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="567a7-103">إذا كنت تتلقي رسالة رفض وصول عند محاولة الاستعراض إلى مركز مسؤول Sharepoint/اندريف ، الرجاء التاكد من [تعيين ترخيص للمستخدم](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="567a7-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="567a7-104">إذا كان لدي المستخدم ترخيص ، يجب أيضا التاكد من [تعيين دور مسؤول](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) يمكنه الوصول إلى مراكز الاداره.</span><span class="sxs-lookup"><span data-stu-id="567a7-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="567a7-105">يمكن ان تحدث هذه المشكلة أيضا عند حذف مستخدم وأعاده إنشائه بنفس الاسم الأساسي للمستخدم (UPN).</span><span class="sxs-lookup"><span data-stu-id="567a7-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="567a7-106">يتم إنشاء الحساب الجديد باستخدام قيمه PUID (معرف فريد لPassport) مختلفه.</span><span class="sxs-lookup"><span data-stu-id="567a7-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="567a7-107">عندما يحاول المستخدم الوصول إلى مجموعه موقع أو اندريف الخاصة بهم ، المستخدم لديه PUID غير صحيحه.</span><span class="sxs-lookup"><span data-stu-id="567a7-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="567a7-108">يتضمن السيناريو الثاني مزامنة الدليل مع الوحدة التنظيمية "Active Directory" (OU).</span><span class="sxs-lookup"><span data-stu-id="567a7-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="567a7-109">إذا كان المستخدمون بالفعل تسجيل الدخول إلى SharePoint ، ومن ثم يتم نقلها إلى OU مختلفه resynced مع SharePoint ، فانها قد تواجه هذه المشكلة.</span><span class="sxs-lookup"><span data-stu-id="567a7-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="567a7-110">لحل هذه المشكلة ، يجب استعاده UPN الأصلي مع الخطوات التالية في المقالة ، [استعاده مستخدم في Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="567a7-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="567a7-111">ملاحظه: إذا لم يتوفر اندريف أو مركز مسؤول SharePoint لعده مستخدمين كان لديهم حق الوصول مسبقا ، قد تكون هناك مشكله خدمه مؤقته.</span><span class="sxs-lookup"><span data-stu-id="567a7-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="567a7-112">[تحقق من لوحه معلومات صحة الخدمة](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="567a7-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


