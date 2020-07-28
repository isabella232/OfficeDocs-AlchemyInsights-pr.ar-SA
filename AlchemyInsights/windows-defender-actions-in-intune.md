---
title: إجراءات Windows Defender في Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1282"
- "6700008"
ms.openlocfilehash: 61a2411ce7c4578ecf2c32943c6a21edbf63eeee
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438789"
---
# <a name="windows-defender-actions-in-intune"></a><span data-ttu-id="3a576-102">إجراءات Windows Defender في Intune</span><span class="sxs-lookup"><span data-stu-id="3a576-102">Windows Defender actions in Intune</span></span>

<span data-ttu-id="3a576-103">يمكن استخدام Intune لتشغيل فحص على الطلب وتحديث توقيع الفيروسات لـ Windows Defender على الأجهزة الفردية.</span><span class="sxs-lookup"><span data-stu-id="3a576-103">Intune can be used to trigger an on-demand scan and virus signature update for Windows Defender on individual devices.</span></span>

<span data-ttu-id="3a576-104">بعد تشغيل إجراء بعيد بنجاح ينعكس النشاط في سجل أحداث Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="3a576-104">After a remote action is successfully triggered the activity is reflected in the Windows Defender event log.</span></span>

<span data-ttu-id="3a576-105">يسمح نهج حماية نقطة النهاية لـ Windows بإنشاء إعدادات إضافية لميزات Windows Defender في Intune وتطبيقها على مجموعات من الأجهزة.</span><span class="sxs-lookup"><span data-stu-id="3a576-105">Windows Endpoint Protection policy allows additional settings for Windows Defender features to be created in Intune and applied to sets of devices.</span></span>

<span data-ttu-id="3a576-106">لمزيد من التفاصيل حول تشغيل إجراءات Windows Defender، راجع [تكوين عمليات المسح الضوئي من Microsoft Defender عند الطلب وتشغيلها](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/run-scan-windows-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="3a576-106">For more details on triggering Windows Defender actions, see [Configure and run on-demand Microsoft Defender Antivirus scans](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/run-scan-windows-defender-antivirus).</span></span>