---
title: حذف المستخدم المعزول من الخادم المحلي
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 537ae7edebfa5a4ab71c2141d549d732ed4f883f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680122"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="3a708-102">حذف المستخدم المعزول من الخادم المحلي</span><span class="sxs-lookup"><span data-stu-id="3a708-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="3a708-103">لأزاله مستخدم معزول ، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="3a708-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="3a708-104">فرض مزامنة الدليل باتباع الإرشادات [الموجودة في الهوية المختلطة باستخدام Azure Active directory ؟](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span><span class="sxs-lookup"><span data-stu-id="3a708-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="3a708-105">للتحقق من مزامنة الدليل ، راجع [ما المقصود بالهوية المختلطة باستخدام Azure Active directory ؟](https://technet.microsoft.com/library/jj151797.aspx).</span><span class="sxs-lookup"><span data-stu-id="3a708-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="3a708-106">إذا كانت الدالة متزامنة بشكل صحيح ولكن حذف كائن Active directory لا يقوم بالنشر في Azure AD ، فقم بازاله الكائن المعزول يدويا باستخدام أحد الوحدة النمطية التالية ل Azure Active directory ل Windows PowerShell:</span><span class="sxs-lookup"><span data-stu-id="3a708-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="3a708-107">أزاله-مسولكونتاكت</span><span class="sxs-lookup"><span data-stu-id="3a708-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="3a708-108">أزاله-مسولجروب</span><span class="sxs-lookup"><span data-stu-id="3a708-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="3a708-109">أزاله-مسولوسير</span><span class="sxs-lookup"><span data-stu-id="3a708-109">Remove-MsolUser</span></span>

    <span data-ttu-id="3a708-110">علي سبيل المثال ، لأزاله معرف المستخدم المعزول john.smith@contoso.com ، الذي تم إنشاؤه في الأصل باستخدام مزامنة الدليل ، قم بتشغيل أمر cmdlet:</span><span class="sxs-lookup"><span data-stu-id="3a708-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="3a708-111">أزاله-مسولوسير-John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="3a708-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>