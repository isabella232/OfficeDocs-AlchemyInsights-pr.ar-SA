---
title: أخطاء مزامنة التسجيل التلقائي لجهاز Apple
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
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714653"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>أخطاء مزامنة التسجيل التلقائي لجهاز Apple

"لقد اكتشفنا ان لديك رمزا مميزا واحدا أو أكثر لجهازي ADE/DEP في حاله خطا. حتى يتم حل حاله الخطا لكل رمز مميز متاثر ، لن تعمل وظيفة ADE في نفس الوقت ".

قد يكون هذا الخطا ظاهرا في عدد من الطرق التي تتضمن:

1. قد لا تتم مزامنة الاجهزه من أبم/ASM إلى Intune
2. قد تفشل تعيينات ملف تعريف التسجيل
3. قد لا تكمل الاجهزه تسجيل ADE بنجاح

تاكد من ان خطا المزامنة الذي تم الإبلاغ عنه في وحده تحكم Intune ضمن **الاجهزه التي > تسجيل الاجهزه التي > تسجيل Apple > الرموز المميزة لبرنامج التسجيل** وراجع الوثائق التالية للاطلاع علي اي تحديث محتمل:

[أخطاء مزامنة أبم/ASM للرموز المميزة لتسجيل الاجهزه التي تعمل بنظام التشغيل iOS/إيبادوس و macOS.](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
