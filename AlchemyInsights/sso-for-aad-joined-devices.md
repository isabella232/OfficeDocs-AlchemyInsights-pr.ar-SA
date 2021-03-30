---
title: Single-Sign على الأجهزة المنضمة إلى Azure Active Directory
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
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404185"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>تسجيل الدخول المفرد للأجهزة المنضمة إلى Azure Active Directory

إذا كانت لديك بيئة Active Directory (AD) المحلية وتريد الانضمام إلى أجهزة الكمبيوتر المنضمة إلى مجال AD إلى Azure AD، يمكنك تنفيذ ذلك من خلال القيام بضم Azure AD المختلط. كيفية: يوفر لك تنفيذ الانضمام إلى [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) المختلط الخطوات ذات الصلة لتنفيذ صلة Azure AD مختلطة في بيئتك.

[تكوين أجهزة Azure AD المتصلة بأجهزة التشغيل Single-Sign باستخدام Windows Hello for Business](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**مشاكل رمز التحديث المميز الأساسي (PRT)** رمز التحديث المميز الأساسي (PRT) هو الأداة الرئيسية لمصادقة Azure AD على أجهزة Windows 10 و Windows Server 2016 والإصدارات الأحدث و iOS و Android. إنه رمز JSON Web Token (JWT) تم إصداره خصيصا ل وسيطي الرمز المميز من جهة Microsoft الأولى لتمكين تسجيل الدخول الفردي (SSO) عبر التطبيقات المستخدمة على هذه الأجهزة. [في ما هو](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)رمز التحديث المميز الأساسي؟ ، سنوفر تفاصيل حول كيفية إصدار PRT، استخدامه، وحمايته على أجهزة Windows 10.

**WamDefaultSet: YES و AzureADPrt: YES** تشير هذه الحقول إلى ما إذا كان المستخدم قد مصادقة على Azure AD بنجاح عند تسجيل الدخول إلى الجهاز. إذا كانت القيم **NO**، فقد تكون مستحقة:

- مفتاح تخزين غير صحيح في TPM المقترن بجهاز عند التسجيل (تحقق من KeySignTest أثناء التشغيل غير المرتد).
- "معرّف تسجيل الدخول البديل"
- لم يتم العثور على وكيل HTTP

استكشاف الأخطاء وإصلاحها باستخدام الأمر dsregcmd - [حالة SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
