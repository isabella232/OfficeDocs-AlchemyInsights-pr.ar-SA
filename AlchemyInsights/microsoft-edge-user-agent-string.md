---
title: Microsoft Edge سلسله عامل المستخدم (سطح المكتب)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003862"
- "6914"
ms.openlocfilehash: b4106dde1e09e0ce07b4b9adc2b2984cc5609c3b
ms.sourcegitcommit: 3c6e777d6679a24108171e9aa3f9379a8d44e001
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/09/2020
ms.locfileid: "49676750"
---
# <a name="microsoft-edge-user-agent-string-desktop"></a><span data-ttu-id="19aae-102">Microsoft Edge سلسله عامل المستخدم (سطح المكتب)</span><span class="sxs-lookup"><span data-stu-id="19aae-102">Microsoft Edge user agent string (Desktop)</span></span>

<span data-ttu-id="19aae-103">يمكن استخدام سلاسل عامل المستخدم (UK-UA&PLATFORM) للكشف عن إصدار مستعرض معين يتم استخدامه علي نظام تشغيل معين.</span><span class="sxs-lookup"><span data-stu-id="19aae-103">User agent (UA) strings can be used to detect what version of a specific browser is being used on a certain operating system.</span></span> <span data-ttu-id="19aae-104">بما في ذلك المستعرضات الأخرى ، يتضمن Microsoft Edge هذه المعلومات في راس صفحه HTTP لعامل المستخدم عندما يقوم بطلب الموقع.</span><span class="sxs-lookup"><span data-stu-id="19aae-104">Like other browsers, Microsoft Edge includes this information in the "User-Agent" HTTP header whenever it makes a request to a site.</span></span> <span data-ttu-id="19aae-105">يمكن أيضا الوصول إلى معلومات إصدارات المستعرض عبر JavaScript عن طريق الاستعلام عن قيمه "أوسيراجينت".</span><span class="sxs-lookup"><span data-stu-id="19aae-105">The browser-version information can also be accessed via JavaScript by querying the value of "navigator.userAgent".</span></span>

<span data-ttu-id="19aae-106">نوصي باستخدام مطوري الويب للكشف عن الميزات كلما أمكن لتحسين مينتينابيليتي التعليمات البرمجية ، وتقليل التعليمات البرمجية لفراجيليتي ، وأزاله مخاطر التعليمات البرمجية بريكاجي في حاله تحديثات سلسله UK-UA&PLATFORM المستقبلية.</span><span class="sxs-lookup"><span data-stu-id="19aae-106">We recommend that web developers make use of feature detection whenever possible to improve code maintainability, reduce code fragility, and eliminate the risk of code breakage in the event of future UA string updates.</span></span>

<span data-ttu-id="19aae-107">للحصول علي مزيد من المعلومات ، راجع [سلسله عامل المستخدم في Microsoft Edge (سطح المكتب)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span><span class="sxs-lookup"><span data-stu-id="19aae-107">For more information, see [Microsoft Edge User Agent String (Desktop)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span></span>