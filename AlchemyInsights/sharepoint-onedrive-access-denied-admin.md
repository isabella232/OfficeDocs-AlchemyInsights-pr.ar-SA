---
title: استكشاف أخطاء رسائل تم رفض الوصول وإصلاحها
ms.author: pebaum
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 4e6fdc6fbf745d1702bf1a7b3474ac82f6662305
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751263"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="be072-102">استكشاف أخطاء الرسائل التي تم رفض الوصول إليها في مركز مسؤول Sharepoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="be072-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="be072-103">إذا كنت تتلقى رسالة تم رفض الوصول عند محاولة الاستعراض إلى مركز مسؤول Sharepoint/OneDrive، الرجاء التأكد من [تعيين ترخيص للمستخدم](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="be072-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="be072-104">إذا كان لدى المستخدم ترخيص، يجب عليك أيضاً التأكد من [تعيين دور مسؤول](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) يمكنه الوصول إلى مراكز المسؤول.</span><span class="sxs-lookup"><span data-stu-id="be072-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="be072-105">يمكن أن تحدث هذه المشكلة أيضًا عند حذف مستخدم وإعادة إنشائه بنفس اسم المستخدم الأساسي (UPN).</span><span class="sxs-lookup"><span data-stu-id="be072-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="be072-106">يتم إنشاء الحساب الجديد باستخدام قيمة PUID (معرف فريد جواز السفر) مختلفة.</span><span class="sxs-lookup"><span data-stu-id="be072-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="be072-107">عندما يحاول المستخدم الوصول إلى مجموعة موقع أو أندريف الخاصة بهم، لدى المستخدم PUID غير صحيح.</span><span class="sxs-lookup"><span data-stu-id="be072-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="be072-108">يتضمن سيناريو ثاني مزامنة الدليل مع وحدة تنظيمية "Active Directory" (OU).</span><span class="sxs-lookup"><span data-stu-id="be072-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="be072-109">إذا قام المستخدمون بالفعل بتسجيل الدخول إلى SharePoint، ثم يتم نقلها إلى وحدة الوحدة التنظيمية مختلفة وإعادة مزامنتها مع SharePoint، فقد تواجه هذه المشكلة.</span><span class="sxs-lookup"><span data-stu-id="be072-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="be072-110">لحل هذه المشكلة، يجب استعادة UPN الأصلي مع الخطوات الموجودة في المقالة [استعادة مستخدم في Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="be072-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="be072-111">ملاحظة: إذا لم يكن مركز مسؤول OneDrive أو SharePoint متوفرًا للعديد من المستخدمين الذين كان لديهم حق الوصول مسبقًا، فقد تكون هناك مشكلة خدمة مؤقتة.</span><span class="sxs-lookup"><span data-stu-id="be072-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="be072-112">[تحقق من لوحة معلومات صحة الخدمة](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="be072-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


