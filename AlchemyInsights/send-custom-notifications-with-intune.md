---
title: إرسال اعلامات مخصصه باستخدام Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720633"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>كيفيه إرسال اعلامات مخصصه إلى مستخدمي نظام التشغيل iOS و Android المدارين

تتم معالجه الإشعارات المخصصة ل Intune بواسطة تطبيق مدخل الشركة علي جهاز المستخدم. ينشئ التطبيق بعد ذلك اعلام الدفع علي ذلك الجهاز.

فيما يلي المتطلبات الاساسيه للجهاز لدعم إيصال اعلامات مخصصه ، ولكي يقوم التطبيق بإنشاء اعلام الدفع:

- يجب ان يكون تطبيق مدخل الشركة مثبتا علي الجهاز.  

- يجب ان يسمح الجهاز لتطبيق مدخل الشركة بإرسال اعلامات الدفع. عند تثبيت التطبيق أو تحديثه ، سيطالب المستخدم بالسماح بالاعلامات.

- يجب ان يتم تثبيت خدمات Google Play علي أجهزه Android.

- يجب ان يتم تسجيل الجهاز باستخدام Intune.

لمزيد من المعلومات ، بما في ذلك كيفيه إرسال رسالة ، راجع [وثائق الميزات](https://docs.microsoft.com/intune/custom-notifications).
