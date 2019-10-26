---
title: ترحيل البريد الإلكتروني من خلال Office 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: e971593b7a67e1bb40243fc762bace6b87a35741
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/25/2019
ms.locfileid: "36745384"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email-using-office-365"></a><span data-ttu-id="2728d-102">إعداد أي جهاز متعدد الوظائف أو تطبيق لإرسال البريد الإلكتروني باستخدام Office 365</span><span class="sxs-lookup"><span data-stu-id="2728d-102">Set up a multifunction device or application to send email using Office 365</span></span>

<span data-ttu-id="2728d-103">للتعرّف على الخيارات والخطوات، اطلع على [كيفية إعداد أي جهاز متعدد الوظائف أو تطبيق لإرسال البريد الإلكتروني باستخدام Office 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span><span class="sxs-lookup"><span data-stu-id="2728d-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Office 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span></span>
  
<span data-ttu-id="2728d-104">**ملاحظة:** إذا كان لديك جهاز أو تطبيق توقف عن العمل مؤخراً، فالرجاء ملاحظة أننا بدأنا مؤخراً [تعطيل تشفير 3DES كما هو مخطط](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption).</span><span class="sxs-lookup"><span data-stu-id="2728d-104">**Note:** If you have a device or application which recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="2728d-105">للاطلاع على الأجهزة المتأثرة، انتقل إلى [تقرير عملاء مصادقة SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="2728d-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="2728d-106">قد تكون الأخطاء الشائعة مشابهة لما يلي: خطأ/فشل المصادقة أو خطأ/فشل TLS أو خطأ خوارزمية التشفير أو عدم تطابق الخوارزمية أو انقطاع الاتصال.</span><span class="sxs-lookup"><span data-stu-id="2728d-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="2728d-107">لحل هذه المشكلة:</span><span class="sxs-lookup"><span data-stu-id="2728d-107">To resolve the issue:</span></span>
 - <span data-ttu-id="2728d-108">**نظام التشغيل Windows Server 2003 IIS SMTP لم يعد يعمل ويتطلب إصدار أحدث من Windows.**</span><span class="sxs-lookup"><span data-stu-id="2728d-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="2728d-109">الرجاء الاتصال بمورّد الجهاز أو التطبيق لمعرفة ما إذا كان التشفير الحديث مدعوماً أو إذا كان هناك تحديث.</span><span class="sxs-lookup"><span data-stu-id="2728d-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
