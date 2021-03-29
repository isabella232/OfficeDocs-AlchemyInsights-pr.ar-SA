---
title: استكشاف الأخطاء في انضمام Azure AD المختلط وإصلاحها
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401894"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a><span data-ttu-id="e0485-102">استكشاف الأخطاء في انضمام Azure AD المختلط وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="e0485-102">Troubleshoot Hybrid Azure AD join</span></span>

<span data-ttu-id="e0485-103">موصى به بشدة تأكد من أن الجهاز يمكنه الوصول إلى نقاط نهاية تسجيل الجهاز ضمن حساب النظام باستخدام البرنامج النصي اختبار اتصال [تسجيل الجهاز](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span><span class="sxs-lookup"><span data-stu-id="e0485-103">Highly Recommended Ensure that a device can access Device Registration endpoints under the system account by using the [Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span></span>

1. <span data-ttu-id="e0485-104">إذا كنت تقوم بإعداد تسجيلات الأجهزة للمرة الأولى، فتأكد من مراجعة I[ntroduction](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) لإدارة الأجهزة في Azure Active Directory للتعرف على كيفية وضع الأجهزة تحت تحكم Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e0485-104">If you are setting up device registrations for the first time, be sure to review I[ntroduction to device management in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) to learn how to get devices under the control of Azure AD.</span></span>
1. <span data-ttu-id="e0485-105">إذا كنت تقوم بتسجيل الأجهزة في Azure AD مباشرة وتسجيلها في Intune، فتأكد من [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) أنك قمت بتكوين [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) وأن الترخيص في مكانه أولا.</span><span class="sxs-lookup"><span data-stu-id="e0485-105">If you are registering devices into Azure AD directly and enrolling them into Intune, be sure that you've [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
1. <span data-ttu-id="e0485-106">تأكد من أنك م مخولا لتنفيذ عمليات في Azure AD و AD في الموقع.</span><span class="sxs-lookup"><span data-stu-id="e0485-106">Ensure that you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="e0485-107">يمكن للمسؤول العام فقط في Azure AD إدارة إعدادات تسجيلات الأجهزة.</span><span class="sxs-lookup"><span data-stu-id="e0485-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="e0485-108">بالإضافة إلى ذلك، إذا كنت تقوم بإعداد التسجيلات التلقائية في Active Directory المحلي، يجب أن تكون مسؤول Active Directory و AD FS (إذا أمكن).</span><span class="sxs-lookup"><span data-stu-id="e0485-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="e0485-109">للحصول على مزيد من التفاصيل حول حل [](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) المشاكل المحتملة باستخدام الصلة المختلطة، راجع استكشاف الأخطاء في "الصلة المختلطة" وإصلاحها لإعداد الأجهزة المختلطة المنضمة إلى Azure AD وإدارتها باستخدام مدخل Azure Ad، راجع إعداد الأجهزة المختلطة المنضمة إلى [Azure AD](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) (المنضمة إلى المجال المحلي) وإدارة الأجهزة باستخدام مدخل [Azure](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="e0485-109">For more details on resolve potential issues with Hybrid join, see [Troubleshoot Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) for set up hybrid Azure AD joined and Manage Devices using Azure Ad portal, see [Set up hybrid Azure AD joined (on-premises domain-joined) devices](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) and [Manage devices using the Azure portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="e0485-110">لحل المشاكل الشائعة في الانضمام إلى Azure Active Directory المختلط (AD)، راجع الأسئلة الشائعة حول الصلة المختلطة ب [Azure AD](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span><span class="sxs-lookup"><span data-stu-id="e0485-110">To resolve common issues with Hybrid Azure Active Directory (AD) join, see [Hybrid Azure AD join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span></span>
