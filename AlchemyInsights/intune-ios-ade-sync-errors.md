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
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="ec3f0-102">أخطاء مزامنة التسجيل التلقائي لجهاز Apple</span><span class="sxs-lookup"><span data-stu-id="ec3f0-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="ec3f0-103">"لقد اكتشفنا ان لديك رمزا مميزا واحدا أو أكثر لجهازي ADE/DEP في حاله خطا.</span><span class="sxs-lookup"><span data-stu-id="ec3f0-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="ec3f0-104">حتى يتم حل حاله الخطا لكل رمز مميز متاثر ، لن تعمل وظيفة ADE في نفس الوقت ".</span><span class="sxs-lookup"><span data-stu-id="ec3f0-104">Until the error state is resolved for each affected token, the ADE functionality will not work for the same”.</span></span>

<span data-ttu-id="ec3f0-105">قد يكون هذا الخطا ظاهرا في عدد من الطرق التي تتضمن:</span><span class="sxs-lookup"><span data-stu-id="ec3f0-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="ec3f0-106">قد لا تتم مزامنة الاجهزه من أبم/ASM إلى Intune</span><span class="sxs-lookup"><span data-stu-id="ec3f0-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="ec3f0-107">قد تفشل تعيينات ملف تعريف التسجيل</span><span class="sxs-lookup"><span data-stu-id="ec3f0-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="ec3f0-108">قد لا تكمل الاجهزه تسجيل ADE بنجاح</span><span class="sxs-lookup"><span data-stu-id="ec3f0-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="ec3f0-109">تاكد من ان خطا المزامنة الذي تم الإبلاغ عنه في وحده تحكم Intune ضمن **الاجهزه التي > تسجيل الاجهزه التي > تسجيل Apple > الرموز المميزة لبرنامج التسجيل** وراجع الوثائق التالية للاطلاع علي اي تحديث محتمل:</span><span class="sxs-lookup"><span data-stu-id="ec3f0-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens** and review the following documentation to see any potential remediation:</span></span>

[<span data-ttu-id="ec3f0-110">أخطاء مزامنة أبم/ASM للرموز المميزة لتسجيل الاجهزه التي تعمل بنظام التشغيل iOS/إيبادوس و macOS.</span><span class="sxs-lookup"><span data-stu-id="ec3f0-110">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
