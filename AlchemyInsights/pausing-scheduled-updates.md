---
title: إيقاف التحديثات المجدولة مؤقتاً
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/30/2020
ms.locfileid: "46554746"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="0dff8-102">إيقاف التحديثات المجدولة مؤقتاً</span><span class="sxs-lookup"><span data-stu-id="0dff8-102">Pausing scheduled updates</span></span>

<span data-ttu-id="0dff8-103">عند إصدار أمر إيقاف مؤقت، لا تقوم الأجهزة بمعالجة الأمر حتى يتم إيداعه في Intune في المرة التالية.</span><span class="sxs-lookup"><span data-stu-id="0dff8-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="0dff8-104">وبسبب هذا، قد تحتوي أجهزتك على:</span><span class="sxs-lookup"><span data-stu-id="0dff8-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="0dff8-105">تثبيت التحديثات المجدولة قبل إيداع.</span><span class="sxs-lookup"><span data-stu-id="0dff8-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="0dff8-106">تم إيقاف التشغيل عند إصدار أمر الإيقاف المؤقت.</span><span class="sxs-lookup"><span data-stu-id="0dff8-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="0dff8-107">في هذه الحالة، عندما تم تشغيل الأجهزة، قد يكون قد قام بتنزيل التحديثات المجدولة وتثبيتها قبل إيداعها.</span><span class="sxs-lookup"><span data-stu-id="0dff8-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>