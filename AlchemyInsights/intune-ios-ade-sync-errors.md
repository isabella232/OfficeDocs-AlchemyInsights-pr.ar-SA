---
title: أخطاء مزامنة تسجيل الجهاز التلقائي في Apple
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
- "9000654"
- "7256"
ms.openlocfilehash: 1664a26b313c4a38c9c6d78cdb89997749ba175fd3dd72f278e99bbd50b0ee84
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013735"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>أخطاء مزامنة تسجيل الجهاز التلقائي في Apple

"لقد اكتشفنا أن لديك رمز ADE/DEP مميز واحد أو أكثر في حالة خطأ. حتى يتم حل حالة الخطأ لكل رمز مميز متأثر، لن تعمل وظيفة ADE كما هو متوقع.".

قد يظهر هذا الخطأ بعدة طرق بما في ذلك:

1. قد لا تتم مزامنة الأجهزة من ABM/ASM إلى Intune
2. قد تفشل تعيينات ملف تعريف التسجيل
3. قد لا تكمل الأجهزة تسجيل ADE بنجاح

تحقق من خطأ المزامنة الذي تم تسجيله في وحدة تحكم Intune ضمن الأجهزة > تسجيل الأجهزة > تسجيل Apple > **المميزة لبرنامج التسجيل.**

أحد الأسباب الأكثر شيوعا لخطأ المزامنة هو انتهاء صلاحية الرمز المميز الحالي. في العديد من الحالات، سيحل تجديد الرمز المميز المتأثر المشكلة.

إذا انتهت صلاحية رمز مميز واحد أو أكثر، فشاهد الوثائق التالية لمساعدتك على تجديدها حسب الاقتضاء:

[تجديد الرمز المميز "تسجيل الجهاز تلقائيا"](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

بالإضافة إلى ذلك، يمكنك الاطلاع على الوثائق التالية لرؤية المعالجة المحتملة لأخطاء أخرى تتسبب في فشل مزامنة الرمز المميز:

[أخطاء مزامنة ABM/ASM ل iOS/iPadOS و macOS الرموز المميزة التلقائية للتسجيل على الجهاز](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[أخطاء مزامنة ABM/ASM ل iOS/iPadOS و macOS الرموز المميزة التلقائية للتسجيل على الجهاز](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
