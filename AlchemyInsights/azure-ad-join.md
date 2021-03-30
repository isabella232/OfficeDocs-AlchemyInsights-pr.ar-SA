---
title: انضمام Azure Active Directory
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9890"
ms.openlocfilehash: 59e3798131956847a61af2416c2e4210199cffa5
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404186"
---
# <a name="azure-active-directory-join"></a><span data-ttu-id="38ffe-102">انضمام Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="38ffe-102">Azure Active Directory join</span></span>

1. <span data-ttu-id="38ffe-103">إذا كنت تقوم بإعداد تسجيلات الأجهزة للمرة الأولى، فتأكد من مراجعة مقدمة حول إدارة الأجهزة في [Azure Active Directory](/azure/active-directory/devices/overview) التي سترشدك إلى كيفية وضع الأجهزة تحت عنصر التحكم إلى Azure AD.</span><span class="sxs-lookup"><span data-stu-id="38ffe-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="38ffe-104">إذا كنت تقوم بتسجيل الأجهزة في Azure AD مباشرة وتسجيلها في Intune، ستحتاج إلى التأكد من [](/mem/intune/fundamentals/licenses-assign) أنك قمت بتكوين [Intune](/mem/intune/enrollment/device-enrollment) وأن يكون الترخيص في مكانه أولا.</span><span class="sxs-lookup"><span data-stu-id="38ffe-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](/mem/intune/enrollment/device-enrollment) and have the [licensing](/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="38ffe-105">تأكد من أنك م مخولا لتنفيذ عمليات في Azure AD.</span><span class="sxs-lookup"><span data-stu-id="38ffe-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="38ffe-106">يمكن للمسؤول العام فقط في Azure AD إدارة إعدادات تسجيلات الأجهزة.</span><span class="sxs-lookup"><span data-stu-id="38ffe-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="38ffe-107">لتنفيذ تنفيذ الانضمام إلى Azure AD، راجع [تخطيط انضمام Azure AD](/azure/active-directory/devices/azureadjoin-plan).</span><span class="sxs-lookup"><span data-stu-id="38ffe-107">To do Azure AD join implementation, see [Plan Azure AD Join](/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="38ffe-108">للحصول على مزيد من التفاصيل حول حل المشاكل الشائعة مع انضمام Azure AD، راجع الأسئلة الشائعة حول انضمام [Azure Ad](/azure/active-directory/devices/faq) وعلى جهاز Windows 10 pro، راجع تعذر الانضمام إلى [جهاز Windows 10 Pro إلى Azure AD -](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)الحاجة إلى الترقية إلى - مجتمع Microsoft .</span><span class="sxs-lookup"><span data-stu-id="38ffe-108">For more details on resolving common issues with Azure AD join, see [Azure Ad Join FAQ](/azure/active-directory/devices/faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900).</span></span>
