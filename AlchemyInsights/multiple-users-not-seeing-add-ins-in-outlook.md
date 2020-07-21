---
title: مستخدمين متعددين لا يرون الوظائف الإضافية في Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197707"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="c6bd4-102">مستخدمين متعددين لا يرون الوظائف الإضافية في Outlook</span><span class="sxs-lookup"><span data-stu-id="c6bd4-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="c6bd4-103">إذا قمت باختبار Outlook الوظائف الإضافية و لا تظهر أي خطوة استكشاف الأخطاء وإصلاحها الأولى استخدم cmdlet **Get-OrganizationConfig** PowerShell الاستعلام _المعلمة AppsForOfficeEnabled._</span><span class="sxs-lookup"><span data-stu-id="c6bd4-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="c6bd4-104">إذا كان الاستعلام بإرجاع قيمة **خطأ**، تعيين هذه المعلمة إلى **True** باستخدام cmdlet **Set-OrganizationConfig** ، لذلك تظهر الوظائف الإضافية كما هو متوقع.</span><span class="sxs-lookup"><span data-stu-id="c6bd4-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="c6bd4-105">لا ننصح تعيين _معلمة AppsForOfficeEnabled_ إلى **False**.</span><span class="sxs-lookup"><span data-stu-id="c6bd4-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="c6bd4-106">تتجاوز قيمة **False** كافة إعدادات دور "الإداري" و"المستخدم" أعلاه وتمنع أي تطبيقات جديدة من أن يتم تنشيطها من قبل أي مستخدم في المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="c6bd4-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="c6bd4-107">لمزيد من المعلومات، راجع [تحديد المسؤولين والمستخدمين الذين يمكنهم تثبيت الوظائف الإضافية لـ Outlook وإدارتها](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span><span class="sxs-lookup"><span data-stu-id="c6bd4-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>