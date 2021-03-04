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
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="191ce-102">أخطاء مزامنة تسجيل الجهاز التلقائي من Apple</span><span class="sxs-lookup"><span data-stu-id="191ce-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="191ce-103">"لقد اكتشفنا أن لديك رمز مميز واحد أو أكثر من رموز ADE/DEP المميزة في حالة خطأ.</span><span class="sxs-lookup"><span data-stu-id="191ce-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="191ce-104">حتى يتم حل حالة الخطأ لكل رمز مميز متأثر، لن تعمل وظيفة ADE كما هو متوقع".</span><span class="sxs-lookup"><span data-stu-id="191ce-104">Until the error state is resolved for each affected token, the ADE functionality will not work as expected.”.</span></span>

<span data-ttu-id="191ce-105">قد يظهر هذا الخطأ بعدة طرق بما في ذلك:</span><span class="sxs-lookup"><span data-stu-id="191ce-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="191ce-106">قد لا تتم مزامنة الأجهزة من ABM/ASM إلى Intune</span><span class="sxs-lookup"><span data-stu-id="191ce-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="191ce-107">قد تفشل تعيينات ملفات تعريف التسجيل</span><span class="sxs-lookup"><span data-stu-id="191ce-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="191ce-108">قد لا تكتمل الأجهزة تسجيل ADE بنجاح</span><span class="sxs-lookup"><span data-stu-id="191ce-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="191ce-109">تحقق من وجود خطأ مزامنة تم تسجيله في وحدة تحكم Intune ضمن **"الأجهزة" > "تسجيل الأجهزة" > تسجيل Apple**> المميزة لبرنامج التسجيل.</span><span class="sxs-lookup"><span data-stu-id="191ce-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens**.</span></span>

<span data-ttu-id="191ce-110">إن انتهاء صلاحية الرمز المميز الحالي هو أحد الأسباب الأكثر شيوعا لخطأ المزامنة.</span><span class="sxs-lookup"><span data-stu-id="191ce-110">One of the most common causes of sync error is expiration of the current token.</span></span> <span data-ttu-id="191ce-111">في العديد من الحالات، سيحل تجديد الرمز المميز المتأثر المشكلة.</span><span class="sxs-lookup"><span data-stu-id="191ce-111">In many cases,renewal of the affected token will resolve the issue.</span></span>

<span data-ttu-id="191ce-112">إذا انتهت صلاحية رمز مميز واحد أو أكثر، فشاهد الوثائق التالية لمساعدتك على تجديدها حسب الاقتضاء:</span><span class="sxs-lookup"><span data-stu-id="191ce-112">If one or more of your tokens has expired,  see the following documentation to help you renew them as appropriate:</span></span>

[<span data-ttu-id="191ce-113">تجديد رمز تسجيل تلقائي لجهاز</span><span class="sxs-lookup"><span data-stu-id="191ce-113">Renew an Automated Device Enrollment token</span></span>](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

<span data-ttu-id="191ce-114">بالإضافة إلى ذلك، يمكنك الاطلاع على الوثائق التالية لمشاهدة المعالجة المحتملة لأخطاء أخرى تتسبب في فشل مزامنة الرمز المميز:</span><span class="sxs-lookup"><span data-stu-id="191ce-114">In addition, you can see the following documentation to see potential remediations for other errors causing token synchronization failures:</span></span>

[<span data-ttu-id="191ce-115">أخطاء مزامنة ABM/ASM ل iOS/iPadOS و macOS التلقائية لرمز تسجيل الجهاز المميز</span><span class="sxs-lookup"><span data-stu-id="191ce-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[<span data-ttu-id="191ce-116">أخطاء مزامنة ABM/ASM ل iOS/iPadOS و macOS التلقائية لرمز تسجيل الجهاز المميز</span><span class="sxs-lookup"><span data-stu-id="191ce-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
