---
title: 2491 تنبيه رسائل البريد الإلكتروني من نهج "تسليم التصيد الاحتيالي بسبب تجاوز المستأجر أو المستخدم"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2b373423cf3e63b76a62465dd62076c023580e94
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544565"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="20e79-102">تنبيه رسائل البريد الإلكتروني من نهج "تسليم التصيد الاحتيالي بسبب تجاوز المستأجر أو المستخدم"</span><span class="sxs-lookup"><span data-stu-id="20e79-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="20e79-103">تم طرح نهج تنبيه افتراضي باسم "تم تسليم التصيد الاحتيالي بسبب تجاوز المستأجر أو المستخدم" للمستأجرين باستخدام تراخيص Microsoft Defender Office 365 P1 و P2.</span><span class="sxs-lookup"><span data-stu-id="20e79-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Microsoft Defender for Office 365 P1 and P2 licenses.</span></span> <span data-ttu-id="20e79-104">إذا تلقيت هذا التنبيه، فيما يلي الخطوات اللازمة للتحقق من ذلك:</span><span class="sxs-lookup"><span data-stu-id="20e79-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="20e79-105">من رسالة التنبيه، انقر فوق **عرض** التنبيهات الانتقال إلى صفحة التنبيهات في مركز التوافق & الأمان. </span><span class="sxs-lookup"><span data-stu-id="20e79-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="20e79-106">حدد التنبيه لرؤية الخيار لعرض قائمة الرسائل **أو** عرض الرسائل **في المستكشف**.</span><span class="sxs-lookup"><span data-stu-id="20e79-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="20e79-107">يأخذك كل من هذين الخيارين إلى تفاصيل الرسالة، التي تتضمن "معرّف الرسالة".</span><span class="sxs-lookup"><span data-stu-id="20e79-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="20e79-108">لاحظ أن الارتباط "مستكشف التهديدات" سيصفي الرسائل التي تتطابق مع معايير التنبيه تلقائيا.</span><span class="sxs-lookup"><span data-stu-id="20e79-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="20e79-109">قد تحتاج إلى ضبط عامل تصفية التاريخ في "مستكشف التهديدات".</span><span class="sxs-lookup"><span data-stu-id="20e79-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="20e79-110">تم تسليم رسالة التصيد الاحتيالي بسبب تجاوز تم تكوينه يدويا:</span><span class="sxs-lookup"><span data-stu-id="20e79-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="20e79-111">مرسل مسموح به أو مجال تم تعيينه بواسطة المستخدم.</span><span class="sxs-lookup"><span data-stu-id="20e79-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="20e79-112">مرسل مسموح به أو مجال تم تعيينه من قبل المسؤول في نهج مكافحة البريد العشوائي.</span><span class="sxs-lookup"><span data-stu-id="20e79-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="20e79-113">عنوان IP مسموح به في نهج عامل تصفية الاتصال.</span><span class="sxs-lookup"><span data-stu-id="20e79-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="20e79-114">قاعدة تدفق البريد (المعروفة أيضا باسم قاعدة النقل) التي تم تكوينها للسماح بالرسائل الواردة.</span><span class="sxs-lookup"><span data-stu-id="20e79-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="20e79-115">إذا كنت تعتقد أنه تم وضع علامة تصيد احتيالي على الرسالة بشكل غير صحيح، فاستخدم Outlook "تقرير الرسالة" الإضافية لإرسال نماذج الرسائل إلى Microsoft. [](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2)</span><span class="sxs-lookup"><span data-stu-id="20e79-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
