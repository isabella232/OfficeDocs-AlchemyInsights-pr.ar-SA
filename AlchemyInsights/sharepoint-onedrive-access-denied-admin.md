---
title: استكشاف أخطاء الوصول الرسائل المرفوضة
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9430b9786b35dda9fb2604fb6ae3c39c8c258d6e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505366"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="a204d-102">استكشاف أخطاء الوصول الرسائل المرفوضة في Sharepoint/OneDrive Admin Center</span><span class="sxs-lookup"><span data-stu-id="a204d-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="a204d-103">إذا كنت تتلقى رسالة رفض الوصول عند محاولة الاستعراض إلى مركز مسؤول Sharepoint/OneDrive، يرجى التأكد من [تعيين ترخيص للمستخدم](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="a204d-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="a204d-104">إذا كان لدى المستخدم ترخيص، يجب عليك [أيضًا](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) التأكد من تعيين دور مسؤول يمكنه الوصول إلى مراكز الإدارة.</span><span class="sxs-lookup"><span data-stu-id="a204d-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="a204d-105">يمكن أن تحدث هذه المشكلة أيضاً عند حذف مستخدم وإعادة إنشائه بنفس اسم المستخدم الرئيسي (UPN).</span><span class="sxs-lookup"><span data-stu-id="a204d-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="a204d-106">يتم إنشاء الحساب الجديد باستخدام قيمة PUID مختلفة (معرف فريد من جواز السفر).</span><span class="sxs-lookup"><span data-stu-id="a204d-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="a204d-107">عندما يحاول المستخدم الوصول إلى مجموعة موقع أو OneDrive الخاص بهم، يكون لدى المستخدم PUID غير صحيح.</span><span class="sxs-lookup"><span data-stu-id="a204d-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="a204d-108">يتضمن سيناريو الثاني مزامنة الدليل مع وحدة تنظيمية "الدليل النشط" (OU).</span><span class="sxs-lookup"><span data-stu-id="a204d-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="a204d-109">إذا قام المستخدمون بتسجيل الدخول بالفعل إلى SharePoint، ثم تم نقلهم إلى OU مختلف وإعادة مزامنتهم مع SharePoint، فقد يواجهون هذه المشكلة.</span><span class="sxs-lookup"><span data-stu-id="a204d-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="a204d-110">لحل هذه المشكلة، يجب استعادة UPN الأصلي مع الخطوات في المقالة استعادة [مستخدم في Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="a204d-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="a204d-111">ملاحظة: إذا كان مركز OneDrive أو SharePoint Admin غير متوفر للعديد من المستخدمين الذين سبق لهم الوصول، فقد تكون هناك مشكلة في الخدمة المؤقتة.</span><span class="sxs-lookup"><span data-stu-id="a204d-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="a204d-112">[تحقق من لوحة معلومات صحة الخدمة](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="a204d-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


