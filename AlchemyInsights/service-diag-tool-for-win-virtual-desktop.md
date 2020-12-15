---
title: أداه تشخيص الخدمة لسطح مكتب Windows الظاهري
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/14/2020
ms.locfileid: "49676935"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="9adc3-102">أداه تشخيص الخدمة لسطح مكتب Windows الظاهري</span><span class="sxs-lookup"><span data-stu-id="9adc3-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="9adc3-103">يوفر Windows Virtual Desktop (وفد) أداه تشخيص تتيح للمسؤولين تحديد الأخطاء عبر واجهه واحده.</span><span class="sxs-lookup"><span data-stu-id="9adc3-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="9adc3-104">تسجل هذه الاداه معلومات ذات صله بالتشخيص عند استخدام وفد بواسطة شخص قام بتعيين دور وفد.</span><span class="sxs-lookup"><span data-stu-id="9adc3-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="9adc3-105">يحتوي كل سجل علي معلومات حول دور وفد المضمن في النشاط ورسائل الخطا التي تظهر اثناء جلسة العمل والمعلومات المتعلقة بالمستاجر والمستخدم.</span><span class="sxs-lookup"><span data-stu-id="9adc3-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="9adc3-106">يمكن تكوين تحليلات سجلات Azure للتقاط سجل النشاط الذي تم إنشاؤه بواسطة أداه التشخيص.</span><span class="sxs-lookup"><span data-stu-id="9adc3-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool.</span></span> <span data-ttu-id="9adc3-107">إليك كيفية تنفيذ ذلك:</span><span class="sxs-lookup"><span data-stu-id="9adc3-107">Here's how:</span></span>

1. <span data-ttu-id="9adc3-108">إنشاء مساحة عمل لتحليلات السجلات باستخدام [مدخل azure](https://go.microsoft.com/fwlink/?linkid=2129500) أو [azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span><span class="sxs-lookup"><span data-stu-id="9adc3-108">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>
1. <span data-ttu-id="9adc3-109">[توصيل أجهزه كمبيوتر Windows ب Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="9adc3-109">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="9adc3-110">احصل علي معرف مساحة العمل والمفتاح الأساسي لمساحة العمل الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="9adc3-110">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="9adc3-111">يحتاج معالج الاعداد إلى هذه المعلومات لتكوين العامل بشكل صحيح وللتاكد من انه يمكنه التواصل مع جهاز عرض Azure.</span><span class="sxs-lookup"><span data-stu-id="9adc3-111">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>
1. <span data-ttu-id="9adc3-112">[دفع بيانات التشخيص إلى مساحة العمل](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="9adc3-112">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="9adc3-113">يمكنك دفع بيانات التشخيص من مستاجر وفد الخاص بك إلى تحليلات السجل لمساحة العمل الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="9adc3-113">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>
1. <span data-ttu-id="9adc3-114">[تحديد المشاكل](https://go.microsoft.com/fwlink/?linkid=2128338) الداخلية أو الخارجية وتشخيصها بالنسبة إلى وفد.</span><span class="sxs-lookup"><span data-stu-id="9adc3-114">[Identify and diagnose issues](https://go.microsoft.com/fwlink/?linkid=2128338) that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="9adc3-115">لمعرفه المزيد حول تكوين أداه تشخيص الخدمة ل وفد ، راجع [استخدام تحليلات السجلات لميزه التشخيص](https://go.microsoft.com/fwlink/?linkid=2128084).</span><span class="sxs-lookup"><span data-stu-id="9adc3-115">To learn more about configuring the service diagnostics tool for WVD, see [Use Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span></span>
