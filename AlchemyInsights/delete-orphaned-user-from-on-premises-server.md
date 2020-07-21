---
title: حذف مستخدم المعزول من خادم محلي
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/20/2020
ms.locfileid: "45197762"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="31b92-102">حذف مستخدم المعزول من خادم محلي</span><span class="sxs-lookup"><span data-stu-id="31b92-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="31b92-103">لإزالة مستخدم المعزول اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="31b92-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="31b92-104">فرض مزامنة الدليل باتباع الإرشادات في [ما هي الهوية المختلطة مع Azure Active Directory؟](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span><span class="sxs-lookup"><span data-stu-id="31b92-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="31b92-105">للتحقق من مزامنة الدليل، راجع [ما هي الهوية المختلطة مع Azure Active Directory؟](https://technet.microsoft.com/library/jj151797.aspx).</span><span class="sxs-lookup"><span data-stu-id="31b92-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="31b92-106">إذا كانت مزامنة دالات بشكل صحيح ولكن لا نشر حذف كائن Active Directory إلى إعلان Azure يدوياً إزالة الكائن المعزول باستخدام أحد الوحدة النمطية "Active Directory أزور" التالية لـ Windows PowerShell cmdlets:</span><span class="sxs-lookup"><span data-stu-id="31b92-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="31b92-107">إزالة-MsolContact</span><span class="sxs-lookup"><span data-stu-id="31b92-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="31b92-108">إزالة-MsolGroup</span><span class="sxs-lookup"><span data-stu-id="31b92-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="31b92-109">إزالة-MsolUser</span><span class="sxs-lookup"><span data-stu-id="31b92-109">Remove-MsolUser</span></span>

    <span data-ttu-id="31b92-110">على سبيل المثال، لإزالة معرف المستخدم المعزول john.smith@contoso.com، تم إنشاؤها في الأصل باستخدام مزامنة الدليل، قم بتشغيل cmdlet:</span><span class="sxs-lookup"><span data-stu-id="31b92-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="31b92-111">إزالة MsolUser -UserPrincipalName John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="31b92-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>