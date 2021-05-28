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
ms.openlocfilehash: 18c68fee514681b2a81c3cfa022c29ce83834f22
ms.sourcegitcommit: 610a5d950cdf488870601762ef52d881e3e22a48
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696909"
---
# <a name="11-call-recording"></a><span data-ttu-id="d7cb2-102">تسجيل المكالمات 1:1</span><span class="sxs-lookup"><span data-stu-id="d7cb2-102">1:1 call recording</span></span>

<span data-ttu-id="d7cb2-103">إذا كان زر بدء **التسجيل** رمادي اللون في مكالمة 1:1، ستحتاج إلى تغيير إعدادات النهج للمستخدم الذي تم التأثير عليه.</span><span class="sxs-lookup"><span data-stu-id="d7cb2-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span>   

<span data-ttu-id="d7cb2-104">بدءا من 31 مايو 2021، سنبدأ بفرض نهج Teams *AllowCloudRecordingForCalls*.</span><span class="sxs-lookup"><span data-stu-id="d7cb2-104">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="d7cb2-105">قبل هذا التغيير، يتم التحكم في تسجيل المكالمات 1:1 بواسطة *AllowCloudRecording Teams* الاجتماع.</span><span class="sxs-lookup"><span data-stu-id="d7cb2-105">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="d7cb2-106">تم توثيق هذا التغيير في منشور مركز الرسائل: [(محدث) مقدمة نهج تسجيل المكالمات 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span><span class="sxs-lookup"><span data-stu-id="d7cb2-106">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="d7cb2-107">*AllowCloudRecordingForCalls*   يتم تعيين خيار نهج الاتصال $False **بشكل** افتراضي.</span><span class="sxs-lookup"><span data-stu-id="d7cb2-107">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="d7cb2-108">إذا كنت تفضل منع جميع المستخدمين من تسجيل المكالمات 1:1، فلا تحتاج إلى اتخاذ أي إجراء.</span><span class="sxs-lookup"><span data-stu-id="d7cb2-108">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="d7cb2-109">لتمكين تسجيل المكالمات لجميع المستخدمين في مكالمات 1:1، استخدم Teams PowerShell لتشغيل cmdlet التالي:</span><span class="sxs-lookup"><span data-stu-id="d7cb2-109">To enable call recording for all users in 1:1 calls use Teams PowerShell to run the following cmdlet:</span></span> 

<span data-ttu-id="d7cb2-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="d7cb2-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="d7cb2-111">بدلا من ذلك، يمكنك إنشاء نهج جديد وتعيين **-AllowCloudRecordingForCalls** $true **وتعيين** هذا النهج للمستخدمين.</span><span class="sxs-lookup"><span data-stu-id="d7cb2-111">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="d7cb2-112">لمزيد من المعلومات، راجع عناصر التحكم في نهج تسجيل المكالمات [1:1 هي (تقريبا!) هنا](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span><span class="sxs-lookup"><span data-stu-id="d7cb2-112">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
