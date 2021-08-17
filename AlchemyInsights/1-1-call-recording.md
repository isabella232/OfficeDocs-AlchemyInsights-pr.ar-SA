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
ms.openlocfilehash: 29383643e6867bca7fd31774a9594b82fdc080bb0e7254141e8c883ad861075e
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/11/2021
ms.locfileid: "57886126"
---
# <a name="11-call-recording"></a>تسجيل المكالمات 1:1

إذا **كان زر** بدء التسجيل رمادي اللون في مكالمة 1:1، ستحتاج إلى تغيير إعدادات النهج للمستخدم الذي تم التأثير عليه. للتحقق من إعداد النهج، قم بتشغيل التشخيص للمستخدم الذي تم التأثير عليه بكتابة **Diag: Teams 1:1 تسجيل** المكالمات أعلاه.     

بدءا من 31 مايو 2021، سنبدأ بفرض نهج Teams *AllowCloudRecordingForCalls*. قبل هذا التغيير، يتم التحكم في تسجيل المكالمات 1:1 بواسطة *AllowCloudRecording Teams* الاجتماع. تم توثيق هذا التغيير في منشور مركز الرسائل: [(محدث) مقدمة نهج تسجيل المكالمات 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).  

*AllowCloudRecordingForCalls*   يتم تعيين خيار نهج الاتصال $False **بشكل** افتراضي. إذا كنت تفضل منع جميع المستخدمين من تسجيل المكالمات 1:1، فلا تحتاج إلى اتخاذ أي إجراء.  

لتمكين تسجيل المكالمات لجميع المستخدمين في المكالمات 1:1 استخدم Teams [PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install) لتشغيل cmdlet التالي: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

بدلا من ذلك، يمكنك إنشاء نهج جديد وتعيين **-AllowCloudRecordingForCalls** $true **وتعيين** هذا النهج للمستخدمين. 

لمزيد من المعلومات، راجع عناصر التحكم في نهج تسجيل المكالمات [1:1 هي (تقريبا!) هنا](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
