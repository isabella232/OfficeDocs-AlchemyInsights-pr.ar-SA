---
title: مستخدمون متعددون لا يريون الوظائف الاضافيه في Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: a0c272f40044795754ed8630e88e00ed14ea6ad7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47729858"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="7340a-102">مستخدمون متعددون لا يريون الوظائف الاضافيه في Outlook</span><span class="sxs-lookup"><span data-stu-id="7340a-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="7340a-103">إذا قمت باختبار وظائف Outlook الاضافيه ولم يظهر اي من الخطوات الاولي ، فاستخدم الأمر **get-organizationconfig** cmdlet للاستعلام عن المعلمة _أبسفوروفيسينابليد_ .</span><span class="sxs-lookup"><span data-stu-id="7340a-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="7340a-104">إذا ارجع الاستعلام قيمه **False**، فقم بتعيين هذه المعلمة إلى **True** باستخدام الأمر **get-organizationconfig** cmdlet ، بحيث تظهر الوظائف الاضافيه كما هو متوقع.</span><span class="sxs-lookup"><span data-stu-id="7340a-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="7340a-105">لا نوصي بتعيين المعلمة _أبسفوروفيسينابليد_ إلى **False**.</span><span class="sxs-lookup"><span data-stu-id="7340a-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="7340a-106">تتجاوز قيمه **False** كل إعدادات ادوار المستخدمين والمسؤولين السابقة وتمنع تنشيط اي تطبيقات جديده من قبل اي مستخدم في المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="7340a-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="7340a-107">لمزيد من المعلومات ، راجع [تحديد المسؤولين والمستخدمين الذين يمكنهم تثبيت الوظائف الاضافيه وأدارتها ل Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span><span class="sxs-lookup"><span data-stu-id="7340a-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>