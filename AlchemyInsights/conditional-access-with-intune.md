---
title: الوصول المشروط مع إينتوني
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 2e778bf4fbdb766700fb24b3405b4ddce89253f7
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/23/2019
ms.locfileid: "32393528"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="a4c59-102">الوصول المشروط مع إينتوني</span><span class="sxs-lookup"><span data-stu-id="a4c59-102">Conditional Access with Intune</span></span>

<span data-ttu-id="a4c59-103">يتطلب استخدام **الوصول المشروط** مع إينتوني ثلاث خطوات:</span><span class="sxs-lookup"><span data-stu-id="a4c59-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="a4c59-104">إنشاء **نهج الوصول الشرطي** بتعريف الموارد التي يتم حمايتها، وما هي الشروط اللازم استيفاؤها للوصول إلى هذه الموارد.</span><span class="sxs-lookup"><span data-stu-id="a4c59-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="a4c59-105">على سبيل المثال، جهاز يجب أن تكون متوافقة مع قبل الوصول إلى البريد الإلكتروني.</span><span class="sxs-lookup"><span data-stu-id="a4c59-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="a4c59-106">إنشاء **نهج التوافق** لتحديد الإعدادات التي يجب استيفاؤها قبل تعتبر متوافقة مع الجهاز.</span><span class="sxs-lookup"><span data-stu-id="a4c59-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="a4c59-107">على سبيل المثال، يجب أن يكون جهاز pin على الأقل 6 أرقام قبل أن يعتبر متوافق.</span><span class="sxs-lookup"><span data-stu-id="a4c59-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="a4c59-108">ضمان **توافق السياسات** و **نهج الوصول الشرطي** تستهدف مجموعات المستخدمين المطلوب.</span><span class="sxs-lookup"><span data-stu-id="a4c59-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="a4c59-109">قد يتطلب هذا إنشاء مجموعات معينة من المستخدمين في Active Directory Azure.</span><span class="sxs-lookup"><span data-stu-id="a4c59-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="a4c59-110">مزيد من المعلومات:</span><span class="sxs-lookup"><span data-stu-id="a4c59-110">Read more:</span></span>
  
- [<span data-ttu-id="a4c59-111">أفضل ممارسات الوصول الشرطي</span><span class="sxs-lookup"><span data-stu-id="a4c59-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="a4c59-112">الشروع في العمل مع "الوصول المشروط"</span><span class="sxs-lookup"><span data-stu-id="a4c59-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

