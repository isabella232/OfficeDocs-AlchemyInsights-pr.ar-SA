---
title: استكشاف أخطاء الوصول إلى الرسائل التي تم رفضها
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767631"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="3c628-102">استكشاف أخطاء الوصول إلى الرسائل التي تم رفضها في مركز أداره Sharepoint/OneDrive وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="3c628-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="3c628-103">إذا تلقيت رسالة تفيد بأنه تم رفض الوصول عند محاولة الاستعراض إلى مركز أداره Sharepoint/OneDrive ، فالرجاء التاكد من [تعيين ترخيص للمستخدم](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="3c628-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="3c628-104">إذا كان لدي المستخدم ترخيص ، فعليك أيضا التاكد من انه قد [تم تعيين دور مسؤول](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) له بحيث يمكنه الوصول إلى مراكز الاداره.</span><span class="sxs-lookup"><span data-stu-id="3c628-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="3c628-105">يمكن ان تحدث هذه المشكلة أيضا عند حذف مستخدم وأعاده إنشائه باستخدام الاسم الأساسي للمستخدم (UPN).</span><span class="sxs-lookup"><span data-stu-id="3c628-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="3c628-106">يتم إنشاء الحساب الجديد باستخدام قيمه مختلفه لبويد (المعرف الفريد ل Passport).</span><span class="sxs-lookup"><span data-stu-id="3c628-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="3c628-107">عندما يحاول المستخدم الوصول إلى مجموعه مواقع مشتركه أو من OneDrive ، فهذا يعني ان المستخدم لديه بويد غير صحيح.</span><span class="sxs-lookup"><span data-stu-id="3c628-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="3c628-108">يتضمن السيناريو الثاني مزامنة الدليل مع الوحدة التنظيمية لخدمه Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="3c628-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="3c628-109">إذا قام المستخدمون بتسجيل الدخول إلى SharePoint بالفعل ، سيتم نقله إلى الوحدة التنظيمية والريسينسيد المختلفة مع SharePoint ، وقد يواجهوا هذه المشكلة.</span><span class="sxs-lookup"><span data-stu-id="3c628-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="3c628-110">لحل هذه المشكلة ، ينبغي عليك استعاده UPN الاصليه باستخدام الخطوات الواردة في المقالة ، [استعاده مستخدم في Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="3c628-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="3c628-111">ملاحظه: إذا لم يكن مركز أداره OneDrive أو SharePoint متوفرا لعده مستخدمين لديهم حق الوصول ، فقد تكون هناك مشكله خدمه مؤقته.</span><span class="sxs-lookup"><span data-stu-id="3c628-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="3c628-112">[تحقق من لوحه معلومات حماية الخدمة](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="3c628-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


