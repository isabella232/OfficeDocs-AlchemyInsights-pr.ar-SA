---
title: رسائل البريد الإلكتروني التنبيه 2491 من النهج 'تجاوز"تسليم فيش" سبب المستأجر أو مستخدم
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391084"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="5d5b8-102">رسائل تنبيه البريد الإلكتروني من نهج 'تجاوز"تسليم فيش" سبب المستأجر أو مستخدم</span><span class="sxs-lookup"><span data-stu-id="5d5b8-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="5d5b8-103">تم توالت نهج تنبيه افتراضي المسمى "فيش التسليم نظراً لتجاوز المستأجر أو المستخدم" للمستأجرين بترخيص Office 365 ATP P1 و P2.</span><span class="sxs-lookup"><span data-stu-id="5d5b8-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="5d5b8-104">إذا تلقيت هذا التنبيه، فيما يلي خطوات للتحقيق:</span><span class="sxs-lookup"><span data-stu-id="5d5b8-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="5d5b8-105">من رسالة التنبيه، انقر فوق **عرض التنبيه** للانتقال إلى صفحة " **التنبيهات** " في & أمان مركز التوافق.</span><span class="sxs-lookup"><span data-stu-id="5d5b8-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="5d5b8-106">حدد التنبيه لرؤية الخيار **عرض الرسائل في "مستكشف"** أو **عرض قائمة الرسائل** .</span><span class="sxs-lookup"><span data-stu-id="5d5b8-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="5d5b8-107">كلا هذين الخيارين تنقلك إلى تفاصيل الرسالة التي تتضمن "معرف الرسالة."</span><span class="sxs-lookup"><span data-stu-id="5d5b8-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="5d5b8-108">لاحظ أن الارتباط التهديد Explorer سيقوم بتصفية الرسائل التي تتطابق مع معايير التنبيه تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="5d5b8-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="5d5b8-109">قد تحتاج إلى ضبط عامل التصفية تاريخ في "مستكشف التهديد".</span><span class="sxs-lookup"><span data-stu-id="5d5b8-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="5d5b8-110">تم تسليم رسالة الاحتيال بسبب تجاوز مكون يدوياً:</span><span class="sxs-lookup"><span data-stu-id="5d5b8-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="5d5b8-111">المسموح بها المرسل أو المجال التي تم تعيينها من قبل المستخدم.</span><span class="sxs-lookup"><span data-stu-id="5d5b8-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="5d5b8-112">المسموح بها المرسل أو المجال تعيين من قبل الإدارة في نهج مكافحة البريد الإلكتروني عشوائي.</span><span class="sxs-lookup"><span data-stu-id="5d5b8-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="5d5b8-113">عنوان IP المسموح بها في نهج تصفية اتصال.</span><span class="sxs-lookup"><span data-stu-id="5d5b8-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="5d5b8-114">بريد تدفق قاعدة (تعرف أيضا باسم قاعدة نقل) الذي تم تكوينه للسماح للرسائل في.</span><span class="sxs-lookup"><span data-stu-id="5d5b8-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="5d5b8-115">إذا كنت تعتقد أنه تم وضع علامة الرسالة بشكل غير صحيح التصيد، استخدام Outlook ["رسالة التقرير" الإضافية](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) لإرسال عينات رسالة إلى Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5d5b8-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
