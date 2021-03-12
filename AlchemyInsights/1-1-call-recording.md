---
title: تسجيل المكالمات 1:1
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733836"
---
# <a name="11-call-recording"></a><span data-ttu-id="22bfb-102">تسجيل المكالمات 1:1</span><span class="sxs-lookup"><span data-stu-id="22bfb-102">1:1 call recording</span></span>

<span data-ttu-id="22bfb-103">يحتاج المسؤولون إلى اتخاذ إجراء الآن لمواصلة السماح للمستخدمين بتسجيل المكالمات 1:1.</span><span class="sxs-lookup"><span data-stu-id="22bfb-103">Administrators need to take action now to continue allowing users to Record 1:1 calls.</span></span>
 
<span data-ttu-id="22bfb-104">اعتبارا من 12 أبريل 2021، سنبدأ بفرض خيار نهج الاتصال الجديد في Teams *AllowCloudRecordingForCalls*.</span><span class="sxs-lookup"><span data-stu-id="22bfb-104">Beginning April 12, 2021, we will start enforcing a new Teams Calling Policy option *AllowCloudRecordingForCalls*.</span></span> 

<span data-ttu-id="22bfb-105">يتم حاليا التحكم في قدرات تسجيل المكالمات 1:1 بواسطة *الخيار AllowCloudRecording* في "سياسات اجتماعات Teams".</span><span class="sxs-lookup"><span data-stu-id="22bfb-105">Currently 1:1 call recording capabilities are controlled by the *AllowCloudRecording* option in Teams Meeting Policies.</span></span> <span data-ttu-id="22bfb-106">إذا تم السماح للمستخدمين بتسجيل اجتماعات Teams، يمكنهم أيضا تسجيل مكالمات 1:1.</span><span class="sxs-lookup"><span data-stu-id="22bfb-106">If your users are allowed to record Teams Meetings they can also record 1:1 calls.</span></span>

<span data-ttu-id="22bfb-107">إذا كنت تفضل منع جميع المستخدمين من تسجيل المكالمات 1:1، لا تحتاج إلى اتخاذ أي إجراء.</span><span class="sxs-lookup"><span data-stu-id="22bfb-107">If you prefer to block all users from recording 1:1 calls, you do not need to take any action.</span></span> <span data-ttu-id="22bfb-108">سيتم تعيين خيار نهج الاتصال *AllowCloudRecordingForCalls* $False بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="22bfb-108">*AllowCloudRecordingForCalls* calling policy option will be $False by default.</span></span>

<span data-ttu-id="22bfb-109">تم توثيق هذا التغيير في منشور مركز الرسائل التالي: [(تم التحديث) 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) مقدمة نهج تسجيل المكالمات لتعيين خيار نهج المكالمات في Teams يجب استخدام [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="22bfb-109">This change is documented in the following Message Center Post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) To set the Teams Calling Policy Option you must use [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span></span>

<span data-ttu-id="22bfb-110">**لتمكين تسجيل المكالمات في 1:1 المكالمات:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span><span class="sxs-lookup"><span data-stu-id="22bfb-110">**To enable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span></span>

<span data-ttu-id="22bfb-111">**لتعطيل تسجيل المكالمات في المكالمات 1:1:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span><span class="sxs-lookup"><span data-stu-id="22bfb-111">**To disable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span></span>

