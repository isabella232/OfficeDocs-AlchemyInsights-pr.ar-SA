---
title: الجهاز في حالة معلقة
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: 224e6e613c306b50e354930bcbe6f43f1c08528766cb6e681b0e9826b2d55a4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53913990"
---
# <a name="device-in-pending-state"></a>الجهاز في حالة معلقة

**المتطلبات الأساسية:**

1. إذا كنت تقوم بإعداد تسجيلات الأجهزة للمرة الأولى، فالرجاء التأكد من مراجعة مقدمة حول إدارة الأجهزة في [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) التي سترشدك إلى كيفية وضع الأجهزة تحت تحكم Azure AD.
2. إذا كنت تقوم بتسجيل الأجهزة في Azure AD مباشرة وتسجيلها في Intune، ستحتاج إلى التأكد من [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) أنك قمت بتكوين [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) وأن يكون الترخيص في مكانه أولا.
3. تأكد من أنك م مخولا لتنفيذ عمليات في Azure AD و AD في الموقع. يمكن للمسؤول العام فقط في Azure AD إدارة إعدادات تسجيلات الأجهزة. بالإضافة إلى ذلك، إذا كنت تقوم بإعداد التسجيلات التلقائية في Active Directory المحلي، يجب أن تكون مسؤول Active Directory و AD FS (إذا أمكن).

تتطلب عملية تسجيل الانضمام إلى Azure AD المختلطة وجود الأجهزة على شبكة الشركة. يعمل أيضا عبر VPN ولكن هناك بعض التحذيرات لذلك. لقد سمعنا أن العملاء بحاجة إلى المساعدة في استكشاف الأخطاء وإصلاحها في عملية تسجيل الانضمام إلى Azure AD المختلطة في ظروف العمل عن بعد.

**بيئة المصادقة السحابية (باستخدام مزامنة كلمة مرور Azure AD أو المصادقة المرورية)**

يعرف تدفق التسجيل هذا أيضا ب "انضمام المزامنة".

فيما يلي تصنيف تفصيلي لما يحدث أثناء عملية التسجيل:

1. Windows 10 عن سجل نقطة اتصال الخدمة (SCP) عند تسجيل المستخدم دخوله إلى الجهاز.

    1. يحاول الجهاز أولا استرداد معلومات المستأجر من SCP من جانب العميل في السجل [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. لمزيد من المعلومات، راجع [المستند](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. إذا فشل، يتواصل الجهاز مع Active Directory في الموقع للحصول على معلومات المستأجر من SCP. للتحقق من SCP، راجع هذا [المستند](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    > [!NOTE]
    > نوصي بتمكين SCP في Active Directory واستخدام SCP من جانب العميل فقط للتحقق من الصحة الأولي.

2. Windows 10 التواصل مع Azure AD ضمن سياق النظام لمصادقة نفسه مقابل Azure AD.

    يمكنك التحقق مما إذا كان الجهاز يمكنه الوصول إلى موارد Microsoft ضمن حساب النظام باستخدام البرنامج النصي [اختبار اتصال تسجيل الجهاز](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. Windows 10 إنشاء شهادة موقعة ذاتيا وتخزينها ضمن كائن الكمبيوتر في Active Directory المحلية. يتطلب هذا الأمر وجود خط البصر في وحدة التحكم بالمجال.

4. يتم مزامنة كائن الجهاز الذي لديه شهادة إلى Azure AD عبر Azure AD الاتصال. تكون دورة المزامنة كل 30 دقيقة بشكل افتراضي، ولكنها تعتمد على تكوين Azure AD الاتصال. لمزيد من المعلومات، راجع هذا [المستند](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. في هذه المرحلة، يجب أن تتمكن من رؤية جهاز الموضوع في حالة "**معلق"** ضمن شفرة الجهاز من مدخل Azure.

6. عند تسجيل دخول المستخدم التالي إلى Windows 10، سيتم إكمال التسجيل.

    > [!NOTE]
    > إذا كنت تستخدم VPN وكان شعار/تسجيل الدخول ينهي اتصال المجال، يمكنك تشغيل التسجيل يدويا. للقيام بذلك:
    >
    > إصدار مطالبة `dsregcmd /join` محلية من المسؤول أو عن بعد عبر PSExec إلى الكمبيوتر الشخصي.
    >
    > على سبيل المثال: `PsExec -s \\win10client01 cmd, dsregcmd /join`

للحصول على المشاكل الشائعة المتعلقة بتسجيل جهاز Azure Active Directory، راجع [الأسئلة الشائعة حول الأجهزة](https://docs.microsoft.com/azure/active-directory/devices/faq).
