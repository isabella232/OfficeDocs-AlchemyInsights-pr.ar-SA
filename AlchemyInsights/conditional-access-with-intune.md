---
title: الوصول المشروط مع اينتوني
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/18/2019
ms.locfileid: "36504981"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="b79ce-102">الوصول المشروط مع اينتوني</span><span class="sxs-lookup"><span data-stu-id="b79ce-102">Conditional Access with Intune</span></span>

<span data-ttu-id="b79ce-103">يتطلب استخدام **الوصول المشروط** مع اينتوني 3 خطوات:</span><span class="sxs-lookup"><span data-stu-id="b79ce-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="b79ce-104">إنشاء **نهج الوصول المشروط** الذي يحدد الموارد المحمية ، وما هي الشروط التي يجب تلبيتها للوصول إلى تلك الموارد.</span><span class="sxs-lookup"><span data-stu-id="b79ce-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="b79ce-105">علي سبيل المثال ، يجب ان يكون الجهاز متوافقا قبل الوصول إلى البريد الكتروني للشركة.</span><span class="sxs-lookup"><span data-stu-id="b79ce-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="b79ce-106">إنشاء **نهج توافق** لتعريف الإعدادات التي يجب ان تتحقق قبل اعتبار الجهاز متوافقا.</span><span class="sxs-lookup"><span data-stu-id="b79ce-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="b79ce-107">علي سبيل المثال ، يجب ان يكون للجهاز دبوس بسته أرقام علي الأقل قبل اعتباره متوافقا.</span><span class="sxs-lookup"><span data-stu-id="b79ce-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="b79ce-108">ضمان استهداف **سياسات التوافق** **وسياسات الوصول المشروط** للمجموعات المطلوبة من المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="b79ce-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="b79ce-109">قد يتطلب هذا إنشاء مجموعات معينه من المستخدمين في "Active Directory Azure".</span><span class="sxs-lookup"><span data-stu-id="b79ce-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="b79ce-110">أقرا المزيد:</span><span class="sxs-lookup"><span data-stu-id="b79ce-110">Read more:</span></span>
  
- [<span data-ttu-id="b79ce-111">أفضل ممارسات الوصول المشروط</span><span class="sxs-lookup"><span data-stu-id="b79ce-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="b79ce-112">الشروع في التشغيل باستخدام الوصول المشروط</span><span class="sxs-lookup"><span data-stu-id="b79ce-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

