---
title: إجراءات Windows Defender في Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1282"
- "6700008"
ms.openlocfilehash: 732b7450121f85416bb0f1868b3722899bee8194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699074"
---
# <a name="windows-defender-actions-in-intune"></a><span data-ttu-id="5c91e-102">إجراءات Windows Defender في Intune</span><span class="sxs-lookup"><span data-stu-id="5c91e-102">Windows Defender actions in Intune</span></span>

<span data-ttu-id="5c91e-103">يمكن استخدام Intune لتشغيل الفحص عند الطلب وتحديث توقيع الفيروسات ل Windows Defender علي الاجهزه الفردية.</span><span class="sxs-lookup"><span data-stu-id="5c91e-103">Intune can be used to trigger an on-demand scan and virus signature update for Windows Defender on individual devices.</span></span>

<span data-ttu-id="5c91e-104">بعد تشغيل الاجراء البعيد بنجاح ، ينعكس النشاط في سجل الاحداث ل Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="5c91e-104">After a remote action is successfully triggered the activity is reflected in the Windows Defender event log.</span></span>

<span data-ttu-id="5c91e-105">يسمح نهج حماية نقاط النهاية ل windows بإنشاء إعدادات اضافيه لميزات Windows Defender في Intune ويتم تطبيقه علي مجموعات من الاجهزه.</span><span class="sxs-lookup"><span data-stu-id="5c91e-105">Windows Endpoint Protection policy allows additional settings for Windows Defender features to be created in Intune and applied to sets of devices.</span></span>

<span data-ttu-id="5c91e-106">للحصول علي مزيد من التفاصيل حول بدء إجراءات Windows Defender ، راجع تكوين عمليات [البحث عن برامج الحماية من الفيروسات وتشغيلها عند الطلب](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/run-scan-windows-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="5c91e-106">For more details on triggering Windows Defender actions, see [Configure and run on-demand Microsoft Defender Antivirus scans](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/run-scan-windows-defender-antivirus).</span></span>