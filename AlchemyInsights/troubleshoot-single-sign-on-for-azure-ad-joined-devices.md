---
title: استكشاف الأخطاء في تسجيل الدخول المفرد للأجهزة المنضمة إلى Azure AD وإصلاحها
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51034799"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>استكشاف الأخطاء في تسجيل الدخول المفرد للأجهزة المنضمة إلى Azure AD وإصلاحها

إذا كانت لديك بيئة Active Directory (AD) المحلية وتريد الانضمام إلى أجهزة الكمبيوتر المنضمة إلى مجال AD إلى Azure AD، يمكنك تنفيذ ذلك من خلال القيام بضم Azure AD المختلط. كيفية: يوفر لك تنفيذ الانضمام إلى [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) المختلط الخطوات ذات الصلة لتنفيذ صلة Azure AD مختلطة في بيئتك.

لمزيد من المعلومات، راجع تكوين الأجهزة المنضمة إلى [Azure AD](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)ل Windows AD Single-Sign تشغيل باستخدام Windows Hello for Business .

**مشاكل رمز التحديث المميز الأساسي (PRT)**

رمز التحديث المميز الأساسي (PRT) هو الأداة الرئيسية لمصادقة Azure AD على أجهزة Windows 10 و Windows Server 2016 والإصدارات الأحدث و iOS و Android. إنه رمز JSON Web Token (JWT) تم إصداره خصيصا ل وسيطي الرمز المميز من جهة Microsoft الأولى لتمكين تسجيل الدخول الفردي (SSO) عبر التطبيقات المستخدمة على هذه الأجهزة. للحصول على تفاصيل حول كيفية إصدار PRT، استخدامه، وحمايته على أجهزة Windows 10، راجع [ما هو رمز التحديث المميز الأساسي؟](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: YES و AzureADPrt: YES**

تشير هذه الحقول إلى ما إذا كان المستخدم قد مصادقة على Azure AD بنجاح عند تسجيل الدخول إلى الجهاز. إذا كانت القيم **لا**، فقد يكون ذلك بسبب:

- مفتاح تخزين غير صحيح في TPM المقترن بجهاز عند التسجيل (تحقق من KeySignTest أثناء التشغيل غير المرتد)
- "معرّف تسجيل الدخول البديل"
- لم يتم العثور على وكيل HTTP

لا استكشاف الأخطاء وإصلاحها في الأجهزة باستخدام الأمر dsregcmd، راجع [حالة SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).
