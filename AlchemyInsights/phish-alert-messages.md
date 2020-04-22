---
title: 2491 رسائل البريد الإلكتروني التنبيه من سياسة "التصيد تم تسليمها بسبب تجاوز المستأجر أو المستخدم"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758892"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="b4e1c-102">رسائل البريد الإلكتروني التنبيه من نهج "التصيد تم تسليمه بسبب تجاوز المستأجر أو المستخدم"</span><span class="sxs-lookup"><span data-stu-id="b4e1c-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="b4e1c-103">تم طرح نهج تنبيه افتراضي يسمى "Phish Delivered بسبب تجاوز المستأجر أو المستخدم" للمستأجرين الذين حصلوا على تراخيص Office 365 ATP P1 وP2.</span><span class="sxs-lookup"><span data-stu-id="b4e1c-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="b4e1c-104">إذا تلقيت هذا التنبيه، فإليك الخطوات للتحقيق:</span><span class="sxs-lookup"><span data-stu-id="b4e1c-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="b4e1c-105">من رسالة التنبيه، انقر فوق **عرض التنبيه** للانتقال إلى صفحة **التنبيهات** في مركز الامتثال & الأمان.</span><span class="sxs-lookup"><span data-stu-id="b4e1c-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="b4e1c-106">حدد التنبيه لرؤية خيار **عرض قائمة الرسائل** أو **عرض الرسائل في Explorer**.</span><span class="sxs-lookup"><span data-stu-id="b4e1c-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="b4e1c-107">كل من هذه الخيارات يأخذك إلى تفاصيل الرسالة، والتي تتضمن معرف الرسالة.</span><span class="sxs-lookup"><span data-stu-id="b4e1c-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="b4e1c-108">لاحظ أن ارتباط مستكشف التهديدات سيقوم تلقائيًا بتصفية الرسائل التي تتطابق مع معايير التنبيه.</span><span class="sxs-lookup"><span data-stu-id="b4e1c-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="b4e1c-109">قد تحتاج إلى ضبط عامل تصفية التاريخ في مستكشف التهديدات.</span><span class="sxs-lookup"><span data-stu-id="b4e1c-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="b4e1c-110">تم تسليم رسالة التصيد بسبب تجاوز تم تكوينه يدويًا:</span><span class="sxs-lookup"><span data-stu-id="b4e1c-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="b4e1c-111">مرسل أو مجال مسموح به تم تعيينه من قبل المستخدم.</span><span class="sxs-lookup"><span data-stu-id="b4e1c-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="b4e1c-112">مرسل أو نطاق مسموح به تم تعيينه من قبل المسؤول في نهج مكافحة الرسائل غير المرغوب فيها.</span><span class="sxs-lookup"><span data-stu-id="b4e1c-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="b4e1c-113">عنوان IP مسموح به في نهج عامل تصفية اتصال.</span><span class="sxs-lookup"><span data-stu-id="b4e1c-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="b4e1c-114">قاعدة تدفق البريد (المعروفة أيضًا باسم قاعدة النقل) التي تم تكوينها للسماح للرسائل بالدخول.</span><span class="sxs-lookup"><span data-stu-id="b4e1c-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="b4e1c-115">إذا كنت تعتقد أنه تم وضع علامة على الرسالة بشكل غير صحيح كـ تصيد، فاستخدم [الوظيفة الإضافية لرسالة تقرير](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) Outlook لإرسال عينات الرسائل إلى Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b4e1c-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
