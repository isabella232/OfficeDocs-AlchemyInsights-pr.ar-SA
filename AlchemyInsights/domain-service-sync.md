---
title: مزامنة خدمه المجال
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: b35d3a402bc08a27a818209385c5666b901fa524
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/15/2021
ms.locfileid: "49884774"
---
# <a name="domain-service-synchronization"></a><span data-ttu-id="285f9-102">مزامنة خدمه المجال</span><span class="sxs-lookup"><span data-stu-id="285f9-102">Domain service synchronization</span></span>

<span data-ttu-id="285f9-103">يمكن ان يتم إنشاء الكائنات وبيانات الاعتماد في المجال المدار ل Azure Active Directory (Azure AD DS) في المجال أو التي تمت مزامنتها من مستاجر Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="285f9-103">Objects and credentials in an Azure Active Directory Domain Services (Azure AD DS) managed domain can either be created locally within the domain, or synchronized from an Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="285f9-104">عندما تقوم بنشر Azure AD DS للمرة الاولي ، يتم تكوين المزامنة التلقائية أحاديه الاتجاه والتي تم بدؤها لاجراء نسخ متماثل للعناصر من Azure AD.</span><span class="sxs-lookup"><span data-stu-id="285f9-104">When you first deploy Azure AD DS, an automatic one-way synchronization is configured and initiated to replicate the objects from Azure AD.</span></span> <span data-ttu-id="285f9-105">تستمر هذه المزامنة أحاديه الاتجاه في العمل في الخلفية لإبقاء المجال المدار في Azure AD DS محدثا بأي تغييرات من Azure AD.</span><span class="sxs-lookup"><span data-stu-id="285f9-105">This one-way synchronization continues to run in the background to keep the Azure AD DS managed domain up-to-date with any changes from Azure AD.</span></span> <span data-ttu-id="285f9-106">لم يحدث اي مزامنة في Azure AD DS مره أخرى.</span><span class="sxs-lookup"><span data-stu-id="285f9-106">No synchronization occurs from Azure AD DS back to Azure AD.</span></span>

<span data-ttu-id="285f9-107">للحصول علي مزيد من التفاصيل حول مزامنة خدمه مجالات Azure Active directory ، راجع [مزامنة خدمه المجال](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span><span class="sxs-lookup"><span data-stu-id="285f9-107">For more details on Azure Active Directory domain service synchronization, see [Domain Service Synchronization](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span></span> 
