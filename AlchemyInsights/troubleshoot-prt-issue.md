---
title: استكشاف مشكلة PRT وإصلاحها
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: fd285d1158d7b358e4c698cf6014422cc2fb536e1fbdf98630bebda359f9c553
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972703"
---
# <a name="troubleshoot-prt-issue"></a>استكشاف مشكلة PRT وإصلاحها

لكي يتمكن أي جهاز من إكمال المصادقة عليه، يجب أن يكون مسجلا بالكامل وفي حالة جيدة وأن يتمكن من الحصول على رمز تحديث مميز أساسي (PRT).

تتطلب عملية تسجيل الانضمام إلى Azure AD المختلطة وجود الأجهزة على شبكة الشركة. يعمل أيضا عبر VPN ولكن هناك بعض التحذيرات لذلك. لقد سمعنا أن العملاء بحاجة إلى المساعدة في استكشاف الأخطاء وإصلاحها في عملية تسجيل الانضمام إلى Azure AD المختلطة في ظروف العمل عن بعد. فيما يلي تصنيف تفصيلي لما يحدث "تحت الغطاء" أثناء عملية التسجيل.

**بيئة المصادقة السحابية (باستخدام مزامنة كلمة مرور Azure AD أو المصادقة المرورية)**

يعرف تدفق التسجيل هذا أيضا ب "انضمام المزامنة".

1. Windows 10 سجل SCP عند تسجيل المستخدم دخوله إلى الجهاز.
    1. يحاول الجهاز أولا استرداد معلومات المستأجر من SCP من جانب العميل في السجل [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. لمزيد من المعلومات، راجع هذا [المستند](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. إذا فشل، يتصل الجهاز ب Active Directory المحلي (AD) للحصول على معلومات المستأجر من نقطة اتصال الخدمة (SCP). للتحقق من SCP، يرجى الرجوع إلى هذا [المستند](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point). 

> [!NOTE]
> نوصي بتمكين SCP في AD واستخدام SCP من جانب العميل فقط للتحقق من الصحة الأولي.

2. Windows 10 التواصل مع Azure AD ضمن سياق النظام لمصادقة نفسه مقابل Azure AD. يمكنك التحقق مما إذا كان الجهاز يمكنه الوصول إلى موارد Microsoft ضمن حساب النظام باستخدام البرنامج النصي اختبار اتصال تسجيل الجهاز.

3. Windows 10 إنشاء شهادة موقعة ذاتيا وتخزينها ضمن كائن الكمبيوتر في AD المحلية. يتطلب هذا الأمر وجود خط البصر في وحدة التحكم بالمجال.

4. يتم مزامنة كائن جهاز لديه شهادة إلى Azure AD عبر Azure AD الاتصال. تكون دورة المزامنة كل 30 دقيقة بشكل افتراضي، ولكنها تعتمد على تكوين Azure AD الاتصال. لمزيد من المعلومات، يرجى الرجوع إلى هذا [المستند](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. في هذه المرحلة، يجب أن تتمكن من رؤية جهاز الموضوع في حالة "معلق" ضمن شفرة الجهاز من مدخل Azure.

6. عند تسجيل دخول المستخدم التالي إلى Windows 10، سيتم إكمال التسجيل. 

> [!NOTE]
> إذا كنت تستخدم VPN وكانت عملية تسجيل الدخول إلى الشعار تنهي اتصال المجال، يمكنك تشغيل التسجيل يدويا:
 1. إصدار dsregcmd /join محليا على مطالبة المسؤول أو عن بعد عبر PSExec إلى الكمبيوتر الشخصي. على سبيل المثال، PsExec -s \\ win10client01 cmd، dsregcmd /join

 2. لمزيد من التفاصيل حول مشاكل "الانضمام المختلط"، راجع استكشاف مشاكل [الأجهزة وإصلاحها](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).
