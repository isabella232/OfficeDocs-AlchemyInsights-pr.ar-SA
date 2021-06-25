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
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/24/2021
ms.locfileid: "53117970"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="9311f-102">إعداد جهاز أو تطبيق متعدد الوظائف لإرسال البريد الإلكتروني</span><span class="sxs-lookup"><span data-stu-id="9311f-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="9311f-103">للتعرّف على الخيارات والخطوات التي لديك، راجع [كيفية إعداد أي جهاز أو تطبيق متعدد الوظائف لإرسال البريد الإلكتروني باستخدام Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="9311f-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="9311f-104">إذا كان لديك جهاز أو تطبيق توقف عن العمل مؤخرا، فإن المشاكل الأكثر شيوعا هي:</span><span class="sxs-lookup"><span data-stu-id="9311f-104">If you have a device or application that recently stopped working, the most common issues are:</span></span>

- <span data-ttu-id="9311f-105">**الأخطاء المتعلقة بالمصادقة أثناء استخدام إرسال عميل SMTP Auth** لقد قمنا مؤخرا بإجراء بعض التغييرات المتعلقة بكيفية عمل مصادقة SMTP.</span><span class="sxs-lookup"><span data-stu-id="9311f-105">**Authentication related errors while using SMTP Auth client submission** We recently made some changes related to how SMTP Authentication works.</span></span> <span data-ttu-id="9311f-106">لمزيد من المعلومات حول كيفية حل المشاكل، راجع قسم المصادقة غير الناجح في إصلاح المشاكل المتعلقة بالطابعات والماسحات الضوئية وتطبيقات LOB التي ترسل البريد الإلكتروني باستخدام Microsoft 365 [أو Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).</span><span class="sxs-lookup"><span data-stu-id="9311f-106">For more information about how to resolve issues, see the authentication unsuccessful section of [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).</span></span>
- <span data-ttu-id="9311f-107">**نحن نقبل إصدار TLS 1.2 فقط مع** إجراء اتصال آمن Office 365 إذا كنت تستخدم اتصال آمن (TLS)، فتأكد من أن جهاز التطبيق يدعم TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="9311f-107">**We accept only the TLS 1.2 version while making a secure connection to Office 365** If you're using Secure connection (TLS), make sure your application device supports TLS 1.2.</span></span> <span data-ttu-id="9311f-108">لمزيد من المعلومات، راجع التحضير ل [TLS 1.2 في](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)Office 365 Office 365 سحابة القطاع الحكومي .</span><span class="sxs-lookup"><span data-stu-id="9311f-108">For more information, see [Preparing for TLS 1.2 in Office 365 and Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span></span>
 
<span data-ttu-id="9311f-109">للحصول على حلول وحلول أخرى، راجع إصلاح المشاكل المتعلقة [بالطابعات](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)والماسحات الضوئية وتطبيقات LOB التي ترسل البريد الإلكتروني باستخدام Microsoft 365 أو Office 365 .</span><span class="sxs-lookup"><span data-stu-id="9311f-109">For other issues and solutions, see [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).</span></span>

<span data-ttu-id="9311f-110">للاطلاع على الأجهزة المتأثرة، انتقل إلى [تقرير عملاء مصادقة SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="9311f-110">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span>

<span data-ttu-id="9311f-111">**ملاحظة:** Exchange Online لا تتلاءم مع سيناريوهات البريد المجمع.</span><span class="sxs-lookup"><span data-stu-id="9311f-111">**Note**: Exchange Online doesn't accommodate bulk-mailing scenarios.</span></span> <span data-ttu-id="9311f-112">لإرسال بريد إلكتروني تجاري مجمع (على سبيل المثال، رسائل العملاء الإخبارية)، يجب استخدام موفرين من جهة خارجية متخصصين في هذه الخدمات.</span><span class="sxs-lookup"><span data-stu-id="9311f-112">To send bulk commercial email (for example, customer newsletters), you should use third-party providers that specialize in these services.</span></span>
