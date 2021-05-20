---
title: استكشاف الأخطاء وإصلاحها ل Microsoft Defender Office 365
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
ms.openlocfilehash: 91d73853d3ea67d6c6954fffb32dd1428e3d9976
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545255"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="6a7ef-102">استكشاف الأخطاء وإصلاحها ل Microsoft Defender Office 365</span><span class="sxs-lookup"><span data-stu-id="6a7ef-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="6a7ef-103">**هل تلاحظ حدوث تأخيرات في تسليم الرسائل؟**</span><span class="sxs-lookup"><span data-stu-id="6a7ef-103">**Do you notice delays in message delivery?**</span></span> <span data-ttu-id="6a7ef-104">استخدم خيار [التسليم الديناميكي](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) في Microsoft Defender Office 365 المرفقات الآمنة.</span><span class="sxs-lookup"><span data-stu-id="6a7ef-104">Use the [Dynamic Delivery](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your Microsoft Defender for Office 365 Safe Attachments policy.</span></span> <span data-ttu-id="6a7ef-105">سيساعد ذلك على تجنب تأخيرات الرسائل أثناء حماية المستلمين من الملفات الضارة.</span><span class="sxs-lookup"><span data-stu-id="6a7ef-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="6a7ef-106">**هل تريد الإبلاغ عن إيجابيات خاطئة أو سلبية خاطئة إلى Microsoft؟**</span><span class="sxs-lookup"><span data-stu-id="6a7ef-106">**Do you want to report false positives or false negatives to Microsoft?**</span></span> <span data-ttu-id="6a7ef-107">استخدم ["مستكشف الواجبات المرسلة".](https://protection.office.com/reportsubmission)</span><span class="sxs-lookup"><span data-stu-id="6a7ef-107">Use [Submissions Explorer](https://protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="6a7ef-108">-\*\* هل تعلم أنه يمكنك تمكين حماية الارتباطات الآمنة للبريد الإلكتروني الداخلي المرسل بين المستلمين داخل مؤسستك؟\*\* اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="6a7ef-108">-\*\* Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?\*\* Follow these steps:</span></span>

  1. <span data-ttu-id="6a7ef-109">انتقل إلى حساب مسؤول عام أو مسؤول الأمان ثم [https://protection.office.com](https://protection.office.com) سجل الدخول إليه.</span><span class="sxs-lookup"><span data-stu-id="6a7ef-109">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="6a7ef-110">في جزء التنقل الأيسر ضمن **إدارة المخاطر،** اختر **الارتباطات الآمنة** \> **ل النهج**.</span><span class="sxs-lookup"><span data-stu-id="6a7ef-110">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="6a7ef-111">في المقطع **النهج التي تنطبق** على قسم المؤسسة بكامله، حدد النهج وانقر فوق **تحرير**.</span><span class="sxs-lookup"><span data-stu-id="6a7ef-111">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="6a7ef-112">ضمن **الإعدادات**، قم بتمكين **تطبيق ارتباطات آمنة على الرسائل المرسلة ضمن المؤسسة**.</span><span class="sxs-lookup"><span data-stu-id="6a7ef-112">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
