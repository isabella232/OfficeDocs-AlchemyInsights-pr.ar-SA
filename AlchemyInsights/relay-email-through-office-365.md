---
title: ترحيل البريد الإلكتروني من خلال Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 56936541c52e56d7aa9b0f5dad7b9a359c5b6185
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809642"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="d559e-102">إعداد جهاز أو تطبيق متعدد الوظائف لإرسال البريد الإلكتروني</span><span class="sxs-lookup"><span data-stu-id="d559e-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="d559e-103">للتعرّف على الخيارات والخطوات التي لديك، راجع [كيفية إعداد أي جهاز أو تطبيق متعدد الوظائف لإرسال البريد الإلكتروني باستخدام Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="d559e-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="d559e-104">**ملاحظة:** إذا كان لديك جهاز أو تطبيق توقف عن العمل مؤخراً، فالرجاء ملاحظة أننا بدأنا مؤخراً [تعطيل تشفير 3DES كما هو مخطط](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption).</span><span class="sxs-lookup"><span data-stu-id="d559e-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="d559e-105">للاطلاع على الأجهزة المتأثرة، انتقل إلى [تقرير عملاء مصادقة SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="d559e-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="d559e-106">قد تكون الأخطاء الشائعة مشابهة لما يلي: خطأ/فشل المصادقة أو خطأ/فشل TLS أو خطأ خوارزمية التشفير أو عدم تطابق الخوارزمية أو انقطاع الاتصال.</span><span class="sxs-lookup"><span data-stu-id="d559e-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="d559e-107">لحل هذه المشكلة:</span><span class="sxs-lookup"><span data-stu-id="d559e-107">To resolve the issue:</span></span>

 - <span data-ttu-id="d559e-108">**نظام التشغيل Windows Server 2003 IIS SMTP لم يعد يعمل ويتطلب إصدار أحدث من Windows.**</span><span class="sxs-lookup"><span data-stu-id="d559e-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="d559e-109">الرجاء الاتصال بمورّد الجهاز أو التطبيق لمعرفة ما إذا كان التشفير الحديث مدعوماً أو إذا كان هناك تحديث.</span><span class="sxs-lookup"><span data-stu-id="d559e-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
