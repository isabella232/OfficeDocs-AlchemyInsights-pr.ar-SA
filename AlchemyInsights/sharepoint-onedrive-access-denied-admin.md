---
title: استكشاف رسائل رفض الوصول وإصلاحها
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707941"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="5fa7b-102">استكشاف الأخطاء في الرسائل التي تم رفض الوصول إليها وإصلاحها في مركز إدارة Sharepoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="5fa7b-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="5fa7b-103">إذا كنت تتلقى رسالة رفض الوصول عند محاولة الاستعراض إلى مركز إدارة Sharepoint/OneDrive، فالرجاء التأكد من تعيين ترخيص [للمستخدم.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)</span><span class="sxs-lookup"><span data-stu-id="5fa7b-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="5fa7b-104">إذا كان لدى المستخدم ترخيص، يجب أيضا [](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) التأكد من تعيين دور مسؤول له يمكنه الوصول إلى مراكز الإدارة.</span><span class="sxs-lookup"><span data-stu-id="5fa7b-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="5fa7b-105">يمكن أن تحدث هذه المشكلة أيضا عند حذف مستخدم ثم إعادة إنشائه بنفس اسم المستخدم الأساسي (UPN).</span><span class="sxs-lookup"><span data-stu-id="5fa7b-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="5fa7b-106">يتم إنشاء الحساب الجديد باستخدام قيمة PUID مختلفة (الم ID الخاص ب جواز السفر).</span><span class="sxs-lookup"><span data-stu-id="5fa7b-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="5fa7b-107">عندما يحاول المستخدم الوصول إلى مجموعة مواقع ويب أو OneDrive الخاص به، يكون لدى المستخدم PUID غير صحيح.</span><span class="sxs-lookup"><span data-stu-id="5fa7b-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="5fa7b-108">يتضمن السيناريو الثاني مزامنة الدليل مع وحدة تنظيمية ل Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="5fa7b-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="5fa7b-109">إذا كان المستخدمون قد سبقوا الدخول إلى SharePoint، ثم تم نقلهم إلى OU آخر ثم إعادة مواصة مع SharePoint، فقد تواجههم هذه المشكلة.</span><span class="sxs-lookup"><span data-stu-id="5fa7b-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="5fa7b-110">لحل هذه المشكلة، يجب استعادة UPN الأصلي باستخدام الخطوات في المقالة، استعادة مستخدم [في Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)</span><span class="sxs-lookup"><span data-stu-id="5fa7b-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="5fa7b-111">ملاحظة: إذا لم يتوفر مركز إدارة OneDrive أو SharePoint لمستخدمين متعددين سبق لهم الوصول إليه، فقد تكون هناك مشكلة مؤقتة في الخدمة.</span><span class="sxs-lookup"><span data-stu-id="5fa7b-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="5fa7b-112">[تحقق من لوحة معلومات "صحة الخدمة".](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="5fa7b-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


