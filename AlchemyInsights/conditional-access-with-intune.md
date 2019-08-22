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
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36504981"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="9d905-102">الوصول المشروط مع إينتوني</span><span class="sxs-lookup"><span data-stu-id="9d905-102">Conditional Access with Intune</span></span>

<span data-ttu-id="9d905-103">يتطلب استخدام **الوصول المشروط** مع إينتوني ثلاث خطوات:</span><span class="sxs-lookup"><span data-stu-id="9d905-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="9d905-104">إنشاء **نهج الوصول الشرطي** بتعريف الموارد التي يتم حمايتها، وما هي الشروط اللازم استيفاؤها للوصول إلى هذه الموارد.</span><span class="sxs-lookup"><span data-stu-id="9d905-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="9d905-105">على سبيل المثال، جهاز يجب أن تكون متوافقة مع قبل الوصول إلى البريد الإلكتروني.</span><span class="sxs-lookup"><span data-stu-id="9d905-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="9d905-106">إنشاء **نهج التوافق** لتحديد الإعدادات التي يجب استيفاؤها قبل تعتبر متوافقة مع الجهاز.</span><span class="sxs-lookup"><span data-stu-id="9d905-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="9d905-107">على سبيل المثال، يجب أن يكون جهاز pin على الأقل 6 أرقام قبل أن يعتبر متوافق.</span><span class="sxs-lookup"><span data-stu-id="9d905-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="9d905-108">ضمان **توافق السياسات** و **نهج الوصول الشرطي** تستهدف مجموعات المستخدمين المطلوب.</span><span class="sxs-lookup"><span data-stu-id="9d905-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="9d905-109">قد يتطلب هذا إنشاء مجموعات معينة من المستخدمين في Active Directory Azure.</span><span class="sxs-lookup"><span data-stu-id="9d905-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="9d905-110">مزيد من المعلومات:</span><span class="sxs-lookup"><span data-stu-id="9d905-110">Read more:</span></span>
  
- [<span data-ttu-id="9d905-111">أفضل ممارسات الوصول الشرطي</span><span class="sxs-lookup"><span data-stu-id="9d905-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="9d905-112">الشروع في العمل مع "الوصول المشروط"</span><span class="sxs-lookup"><span data-stu-id="9d905-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

