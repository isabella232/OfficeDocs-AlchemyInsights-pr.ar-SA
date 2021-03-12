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
# <a name="11-call-recording"></a>تسجيل المكالمات 1:1

يحتاج المسؤولون إلى اتخاذ إجراء الآن لمواصلة السماح للمستخدمين بتسجيل المكالمات 1:1.
 
اعتبارا من 12 أبريل 2021، سنبدأ بفرض خيار نهج الاتصال الجديد في Teams *AllowCloudRecordingForCalls*. 

يتم حاليا التحكم في قدرات تسجيل المكالمات 1:1 بواسطة *الخيار AllowCloudRecording* في "سياسات اجتماعات Teams". إذا تم السماح للمستخدمين بتسجيل اجتماعات Teams، يمكنهم أيضا تسجيل مكالمات 1:1.

إذا كنت تفضل منع جميع المستخدمين من تسجيل المكالمات 1:1، لا تحتاج إلى اتخاذ أي إجراء. سيتم تعيين خيار نهج الاتصال *AllowCloudRecordingForCalls* $False بشكل افتراضي.

تم توثيق هذا التغيير في منشور مركز الرسائل التالي: [(تم التحديث) 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) مقدمة نهج تسجيل المكالمات لتعيين خيار نهج المكالمات في Teams يجب استخدام [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).

**لتمكين تسجيل المكالمات في 1:1 المكالمات:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True

**لتعطيل تسجيل المكالمات في المكالمات 1:1:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False

