---
title: الوصول المشروط مع Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706008"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="d76b0-102">الوصول المشروط مع Intune</span><span class="sxs-lookup"><span data-stu-id="d76b0-102">Conditional Access with Intune</span></span>

<span data-ttu-id="d76b0-103">يتطلب استخدام **الوصول الشرطي** مع Intune 3 خطوات:</span><span class="sxs-lookup"><span data-stu-id="d76b0-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="d76b0-104">إنشاء **نهج الوصول المشروط** الذي يحدد الموارد التي يتم حمايتها، والشروط التي يجب الوفاء بها للوصول إلى تلك الموارد.</span><span class="sxs-lookup"><span data-stu-id="d76b0-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="d76b0-105">على سبيل المثال، يجب أن يكون الجهاز متوافقًا قبل الوصول إلى البريد الإلكتروني للشركة.</span><span class="sxs-lookup"><span data-stu-id="d76b0-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="d76b0-106">إنشاء **نهج الامتثال** لتعريف الإعدادات التي يجب الوفاء بها قبل اعتبار الجهاز متوافقًا.</span><span class="sxs-lookup"><span data-stu-id="d76b0-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="d76b0-107">على سبيل المثال، يجب أن يحتوي الجهاز على دبوس لا يقل عن 6 أرقام قبل اعتباره متوافقًا.</span><span class="sxs-lookup"><span data-stu-id="d76b0-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="d76b0-108">ضمان توجيه كل من **سياسات الامتثال** وسياسات الوصول **المشروط** إلى المجموعات المطلوبة من المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="d76b0-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="d76b0-109">قد يتطلب هذا إنشاء مجموعات معينة من المستخدمين في Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d76b0-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="d76b0-110">اقرأ المزيد:</span><span class="sxs-lookup"><span data-stu-id="d76b0-110">Read more:</span></span>
  
- [<span data-ttu-id="d76b0-111">أفضل ممارسات الوصول المشروط</span><span class="sxs-lookup"><span data-stu-id="d76b0-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="d76b0-112">البدء باستخدام الوصول المشروط</span><span class="sxs-lookup"><span data-stu-id="d76b0-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

