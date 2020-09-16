---
title: 2491 رسائل البريد الكتروني الخاصة بالتنبيه من النهج "تم التسليم بالفيش بسبب المستاجر أو تجاوز المستخدم"
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
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728598"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="96adb-102">تنبيه رسائل البريد الكتروني من النهج "تم تسليم الفيش بسبب المستاجر أو تجاوز المستخدم"</span><span class="sxs-lookup"><span data-stu-id="96adb-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="96adb-103">تم سحب نهج تنبيه افتراضي يحمل الاسم "فيش يتم تسليمه بالنظر إلى المستاجر أو تجاوز المستخدم" إلى المستاجرين باستخدام تراخيص Office 365 ATP P1 و P2.</span><span class="sxs-lookup"><span data-stu-id="96adb-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="96adb-104">إذا تلقيت هذا التنبيه ، فاليك الخطوات التي يجب التحقق منها:</span><span class="sxs-lookup"><span data-stu-id="96adb-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="96adb-105">من رسالة التنبيه ، انقر فوق **عرض التنبيه** للانتقال إلى صفحه **التنبيات** في مركز توافق & الأمان.</span><span class="sxs-lookup"><span data-stu-id="96adb-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="96adb-106">حدد التنبيه لرؤية الخيار الخاص **بعرض قائمه الرسائل** أو **عرض الرسائل في "المستكشف**".</span><span class="sxs-lookup"><span data-stu-id="96adb-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="96adb-107">يقوم كل من هذين الخيارين بنقلك إلى تفاصيل الرسالة ، التي تتضمن معرف الرسالة.</span><span class="sxs-lookup"><span data-stu-id="96adb-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="96adb-108">لاحظ ان الارتباط "مستكشف المخاطر" سيقوم تلقائيا بتصفية الرسائل التي تتطابق مع معايير التنبيه.</span><span class="sxs-lookup"><span data-stu-id="96adb-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="96adb-109">قد تحتاج إلى ضبط عامل تصفيه التاريخ في مستكشف التهديد.</span><span class="sxs-lookup"><span data-stu-id="96adb-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="96adb-110">تم تسليم رسالة التصيد الاحتيالي بسبب تجاوز تم تكوينه يدويا:</span><span class="sxs-lookup"><span data-stu-id="96adb-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="96adb-111">المرسل أو المجال الذي تم تعيينه من قبل المستخدم.</span><span class="sxs-lookup"><span data-stu-id="96adb-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="96adb-112">المرسل أو المجال الذي تم تعيينه بواسطة المسؤول في نهج الحماية من البريد العشوائي.</span><span class="sxs-lookup"><span data-stu-id="96adb-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="96adb-113">عنوان IP مسموح به في نهج عامل تصفيه الاتصال.</span><span class="sxs-lookup"><span data-stu-id="96adb-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="96adb-114">قاعده تدفق البريد (المعروفة أيضا باسم قاعده النقل) المكونة للسماح بالرسائل في.</span><span class="sxs-lookup"><span data-stu-id="96adb-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="96adb-115">إذا كنت تعتقد انه تم وضع علامة علي الرسالة بشكل غير صحيح كفيش ، فاستخدم [الوظيفة الاضافيه "رسالة التقرير](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) " في Outlook لإرسال نماذج الرسائل إلى Microsoft.</span><span class="sxs-lookup"><span data-stu-id="96adb-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
