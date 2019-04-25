---
title: تحديد إعادة توجيه بريد إلكتروني خارجي على علب البريد الموجودة في سجلات التدقيق
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 7fb2c161c558a7eb961f86ca2b86e33750d902fd
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/23/2019
ms.locfileid: "32417199"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="66f86-102">تحديد متى يتم تكوين إعادة توجيه البريد الإلكتروني الخارجي على علب البريد</span><span class="sxs-lookup"><span data-stu-id="66f86-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="66f86-103">عندما يقوم مستخدم بتكوين إعادة توجيه البريد الإلكتروني الخارجي على علبة بريد، يتم تدوين النشاط كجزء من cmdlet **مجموعة-علبة البريد** .</span><span class="sxs-lookup"><span data-stu-id="66f86-103">When a user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="66f86-104">يمكنك مشاهدة النشاط باستخدام البحث سجل التدقيق في & أمان مركز التوافق.</span><span class="sxs-lookup"><span data-stu-id="66f86-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="66f86-105">تسجيل الدخول إلى [مركز التوافق ل Office الأمن 365 &](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="66f86-105">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="66f86-106">انقر فوق **البحث والتحقيق** ، وحدد **البحث في سجل التدقيق**.</span><span class="sxs-lookup"><span data-stu-id="66f86-106">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="66f86-107">حدد نطاق التواريخ في حقول **تاريخ البدء** **وتاريخ الانتهاء** .</span><span class="sxs-lookup"><span data-stu-id="66f86-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="66f86-108">لا تحتاج إلى تحديد اسم مستخدم.</span><span class="sxs-lookup"><span data-stu-id="66f86-108">You don't need to specify a username.</span></span> <span data-ttu-id="66f86-109">تحقق من تعيين حقل **الأنشطة** **إظهار النتائج لكافة الأنشطة**.</span><span class="sxs-lookup"><span data-stu-id="66f86-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="66f86-110">انقر فوق **بحث**.</span><span class="sxs-lookup"><span data-stu-id="66f86-110">Click **Search**.</span></span>

<span data-ttu-id="66f86-111">في النتائج، انقر فوق **عامل تصفية النتائج** واكتب **علبة مجموعة** في المربع النشاط.</span><span class="sxs-lookup"><span data-stu-id="66f86-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="66f86-112">حدد سجل تدقيق في النتائج.</span><span class="sxs-lookup"><span data-stu-id="66f86-112">Select an audit record in the results.</span></span> <span data-ttu-id="66f86-113">في القائمة الفرعية **تفاصيل** ، انقر فوق **مزيد من المعلومات**.</span><span class="sxs-lookup"><span data-stu-id="66f86-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="66f86-114">يجب عليك مراجعة تفاصيل كل سجل التدوين لتحديد حالة تتعلق بالنشاط إرسال البريد الإلكتروني.</span><span class="sxs-lookup"><span data-stu-id="66f86-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="66f86-115">**ObjectId**: قيمة الاسم المستعار علبة البريد التي تم تعديلها.</span><span class="sxs-lookup"><span data-stu-id="66f86-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="66f86-116">**المعلمات**: _فورواردينجسمتبادريس_ يشير إلى عنوان البريد الإلكتروني الهدف.</span><span class="sxs-lookup"><span data-stu-id="66f86-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="66f86-117">**اسم المستخدم**: المستخدم الذي قام بتكوين إعادة توجيه البريد الإلكتروني في صندوق البريد في ميدان **ObjectId** .</span><span class="sxs-lookup"><span data-stu-id="66f86-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="66f86-118">لمزيد من المعلومات، راجع [تحديد الذي قام بإعداد علبة بريد إرسال البريد الإلكتروني](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="66f86-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
