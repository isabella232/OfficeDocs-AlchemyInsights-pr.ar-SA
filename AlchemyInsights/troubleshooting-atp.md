---
title: استكشاف أخطاء Microsoft Defender ل Office 365 وإصلاحها
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 2c9543660056ebc02b0bd297f619f20fa6820093
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801430"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="10b24-102">استكشاف أخطاء Microsoft Defender ل Office 365 وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="10b24-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="10b24-103">هل تلاحظ تاخير في تسليم الرسائل ؟</span><span class="sxs-lookup"><span data-stu-id="10b24-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="10b24-104">استخدم خيار [التسليم الديناميكي](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) في نهج المرفقات الامنه ل ATP.</span><span class="sxs-lookup"><span data-stu-id="10b24-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="10b24-105">سيساعدك هذا في تجنب تاخير الرسائل اثناء حماية المستلمين من الملفات الضارة.</span><span class="sxs-lookup"><span data-stu-id="10b24-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="10b24-106">هل تريد الإبلاغ عن false بوسيتيفيس أو خطا في النيجاتيف إلى Microsoft ؟</span><span class="sxs-lookup"><span data-stu-id="10b24-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="10b24-107">استخدم هذا [الارتباط](https://www.microsoft.com/wdsi/filesubmission/) لإرسال الملفات لتحليلها.</span><span class="sxs-lookup"><span data-stu-id="10b24-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="10b24-108">هل تعلم انه بإمكانك تمكين حماية الارتباطات الامنه للبريد الكتروني الذي يتم إرساله بين المستلمين في مؤسستك ؟</span><span class="sxs-lookup"><span data-stu-id="10b24-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="10b24-109">اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="10b24-109">Follow these steps:</span></span>

  1. <span data-ttu-id="10b24-110">انتقل إلى [https://protection.office.com](https://protection.office.com) وقم بتسجيل الدخول باستخدام حساب مسؤول الأمان أو المسؤول العام.</span><span class="sxs-lookup"><span data-stu-id="10b24-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="10b24-111">في جزء التنقل الأيمن ضمن **أداره التهديدات** ، اختر **Policy** \> **الارتباطات الامنه** للنهج.</span><span class="sxs-lookup"><span data-stu-id="10b24-111">In the left navigation pane under **Threat management** , choose **Policy** \> **Safe Links** .</span></span>

  3. <span data-ttu-id="10b24-112">في **النهج التي تنطبق علي القسم المؤسسة بالبالكامل** ، حدد النهج وانقر فوق **تحرير** .</span><span class="sxs-lookup"><span data-stu-id="10b24-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit** .</span></span>

  4. <span data-ttu-id="10b24-113">ضمن **إعدادات** ، قم بتمكين **تطبيق الارتباطات الامنه علي الرسائل المرسلة داخل المؤسسة** .</span><span class="sxs-lookup"><span data-stu-id="10b24-113">Under **Settings** , enable **Apply safe links to messages sent within the organization** .</span></span>
