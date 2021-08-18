---
title: إرسال إعلامات مخصصة باستخدام Intune
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
ms.openlocfilehash: 58acaa29f9d0b066cc7be6f6ee57b1806d0e8812b194e20166b133b7715226a8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086151"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>كيفية إرسال إعلامات مخصصة إلى مستخدمي أجهزة iOS وAndroid المدارة

تتم معالجة الإعلامات المخصصة ل Intune بواسطة تطبيق Company Portal على جهاز المستخدم. بعد ذلك، ينشئ التطبيق إعلام الدفع على هذا الجهاز.

فيما يلي المتطلبات الأساسية للجهاز لدعم تلقي الإعلامات المخصصة، ومن أجل أن ينشئ التطبيق إعلام الدفع:

- يجب أن يكون تطبيق Company Portal مثبتا على الجهاز.  

- يجب أن يسمح الجهاز لتطبيق Company Portal بإرسال الإعلامات. عند تثبيت التطبيق أو تحديثه، سيطالب المستخدم بترك الإعلامات.

- يجب أن تكون Google Play Services مثبتا على أجهزة Android.

- يجب أن يكون الجهاز مسجلا في Intune.

لمزيد من المعلومات بما في ذلك كيفية إرسال رسالة، راجع [وثائق الميزات](https://docs.microsoft.com/intune/custom-notifications).
