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
ms.openlocfilehash: ffdaca1ba45a6f273809dbe50a7c40e8610193e1
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666503"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email-using-office-365"></a><span data-ttu-id="0d003-102">إعداد أي جهاز متعدد الوظائف أو تطبيق لإرسال البريد الإلكتروني باستخدام Office 365</span><span class="sxs-lookup"><span data-stu-id="0d003-102">Set up a multifunction device or application to send email using Office 365</span></span>

<span data-ttu-id="0d003-103">للتعرّف على الخيارات والخطوات، اطلع على [كيفية إعداد أي جهاز متعدد الوظائف أو تطبيق لإرسال البريد الإلكتروني باستخدام Office 365](https://support.office.com/article/69f58e99-c550-4274-ad18-c805d654b4c4).</span><span class="sxs-lookup"><span data-stu-id="0d003-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Office 365](https://support.office.com/article/69f58e99-c550-4274-ad18-c805d654b4c4).</span></span>
  
<span data-ttu-id="0d003-104">**ملاحظة:** إذا كان لديك جهاز أو تطبيق توقف عن العمل مؤخراً، فالرجاء ملاحظة أننا بدأنا مؤخراً [تعطيل تشفير 3DES كما هو مخطط](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption).</span><span class="sxs-lookup"><span data-stu-id="0d003-104">**Note:** If you have a device or application which recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="0d003-105">للاطلاع على الأجهزة المتأثرة، انتقل إلى [تقرير عملاء مصادقة SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="0d003-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="0d003-106">قد تكون الأخطاء الشائعة مشابهة لما يلي: خطأ/فشل المصادقة أو خطأ/فشل TLS أو خطأ خوارزمية التشفير أو عدم تطابق الخوارزمية أو انقطاع الاتصال.</span><span class="sxs-lookup"><span data-stu-id="0d003-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="0d003-107">لحل هذه المشكلة:</span><span class="sxs-lookup"><span data-stu-id="0d003-107">To resolve the issue:</span></span>
 - <span data-ttu-id="0d003-108">**نظام التشغيل Windows Server 2003 IIS SMTP لم يعد يعمل ويتطلب إصدار أحدث من Windows.**</span><span class="sxs-lookup"><span data-stu-id="0d003-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="0d003-109">الرجاء الاتصال بمورّد الجهاز أو التطبيق لمعرفة ما إذا كان التشفير الحديث مدعوماً أو إذا كان هناك تحديث.</span><span class="sxs-lookup"><span data-stu-id="0d003-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
