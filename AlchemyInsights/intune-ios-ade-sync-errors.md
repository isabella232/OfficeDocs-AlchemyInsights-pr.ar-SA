---
title: أخطاء مزامنة تسجيل الجهاز التلقائي من Apple
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
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448909"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>أخطاء مزامنة تسجيل الجهاز التلقائي من Apple

"لقد اكتشفنا أن لديك رمز مميز واحد أو أكثر من رموز ADE/DEP المميزة في حالة خطأ. حتى يتم حل حالة الخطأ لكل رمز مميز متأثر، لن تعمل وظيفة ADE كما هو متوقع".

قد يظهر هذا الخطأ بعدة طرق بما في ذلك:

1. قد لا تتم مزامنة الأجهزة من ABM/ASM إلى Intune
2. قد تفشل تعيينات ملفات تعريف التسجيل
3. قد لا تكتمل الأجهزة تسجيل ADE بنجاح

تحقق من وجود خطأ مزامنة تم تسجيله في وحدة تحكم Intune ضمن **"الأجهزة" > "تسجيل الأجهزة" > تسجيل Apple**> المميزة لبرنامج التسجيل.

إن انتهاء صلاحية الرمز المميز الحالي هو أحد الأسباب الأكثر شيوعا لخطأ المزامنة. في العديد من الحالات، سيحل تجديد الرمز المميز المتأثر المشكلة.

إذا انتهت صلاحية رمز مميز واحد أو أكثر، فشاهد الوثائق التالية لمساعدتك على تجديدها حسب الاقتضاء:

[تجديد رمز تسجيل تلقائي لجهاز](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

بالإضافة إلى ذلك، يمكنك الاطلاع على الوثائق التالية لمشاهدة المعالجة المحتملة لأخطاء أخرى تتسبب في فشل مزامنة الرمز المميز:

[أخطاء مزامنة ABM/ASM ل iOS/iPadOS و macOS التلقائية لرمز تسجيل الجهاز المميز](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[أخطاء مزامنة ABM/ASM ل iOS/iPadOS و macOS التلقائية لرمز تسجيل الجهاز المميز](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
