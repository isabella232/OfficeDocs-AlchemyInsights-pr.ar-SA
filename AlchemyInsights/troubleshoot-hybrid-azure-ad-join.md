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
ms.openlocfilehash: 23da360965a5972e328844d505698c91ece61788240d8fdb8909fff3a7ef0d7f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939258"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>استكشاف الأخطاء في انضمام Azure AD المختلط وإصلاحها

موصى به بشدة تأكد من أن الجهاز يمكنه الوصول إلى نقاط نهاية تسجيل الجهاز ضمن حساب النظام باستخدام البرنامج النصي اختبار اتصال [تسجيل الجهاز](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).

1. إذا كنت تقوم بإعداد تسجيلات الأجهزة للمرة الأولى، فتأكد من مراجعة I[ntroduction](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) لإدارة الأجهزة في Azure Active Directory للتعرف على كيفية وضع الأجهزة تحت تحكم Azure AD.
1. إذا كنت تقوم بتسجيل الأجهزة في Azure AD مباشرة وتسجيلها في Intune، فتأكد من [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) أنك قمت بتكوين [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) وأن الترخيص في مكانه أولا.
1. تأكد من أنك م مخولا لتنفيذ عمليات في Azure AD و AD في الموقع. يمكن للمسؤول العام فقط في Azure AD إدارة إعدادات تسجيلات الأجهزة. بالإضافة إلى ذلك، إذا كنت تقوم بإعداد التسجيلات التلقائية في Active Directory المحلي، يجب أن تكون مسؤول Active Directory و AD FS (إذا أمكن).

للحصول على مزيد من التفاصيل حول حل [](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) المشاكل المحتملة باستخدام الصلة المختلطة، راجع استكشاف الأخطاء في "الصلة المختلطة" وإصلاحها لإعداد الأجهزة المختلطة المنضمة إلى Azure AD وإدارتها باستخدام مدخل Azure Ad، راجع إعداد الأجهزة المختلطة المنضمة إلى [Azure AD](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) (المنضمة إلى المجال المحلي) وإدارة الأجهزة باستخدام مدخل [Azure](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

لحل المشاكل الشائعة في الانضمام إلى Azure Active Directory المختلط (AD)، راجع الأسئلة الشائعة حول الصلة المختلطة ب [Azure AD](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).
