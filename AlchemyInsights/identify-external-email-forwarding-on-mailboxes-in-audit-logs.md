---
title: تحديد إعادة توجيه بريد إلكتروني خارجي على علب البريد الموجودة في سجلات التدقيق
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 7defd0902e8c8bebae9c7bfee72c3199cbc1909f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539088"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="58352-102">تحديد متى يتم تكوين إعادة توجيه البريد الإلكتروني الخارجي على علب البريد</span><span class="sxs-lookup"><span data-stu-id="58352-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="58352-103">عند تكوين مستخدم Office 365 إعادة توجيه البريد الإلكتروني الخارجي على علبة بريد، يتم تدوين النشاط كجزء من cmdlet **مجموعة-علبة البريد** .</span><span class="sxs-lookup"><span data-stu-id="58352-103">When an Office 365  user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="58352-104">يمكنك مشاهدة النشاط باستخدام البحث سجل التدقيق في & أمان مركز التوافق.</span><span class="sxs-lookup"><span data-stu-id="58352-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="58352-105">تسجيل الدخول إلى [مركز التوافق & الأمن 365 Office](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="58352-105">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="58352-106">انتقل إلى **بحث** > صفحة**البحث في سجل التدقيق** .</span><span class="sxs-lookup"><span data-stu-id="58352-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="58352-107">حدد نطاق التواريخ في حقول **تاريخ البدء** **وتاريخ الانتهاء** .</span><span class="sxs-lookup"><span data-stu-id="58352-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="58352-108">لا تحتاج إلى تحديد اسم مستخدم.</span><span class="sxs-lookup"><span data-stu-id="58352-108">You don't need to specify a username.</span></span> <span data-ttu-id="58352-109">تحقق من تعيين حقل **الأنشطة** **إظهار النتائج لكافة الأنشطة**.</span><span class="sxs-lookup"><span data-stu-id="58352-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="58352-110">انقر فوق **بحث**.</span><span class="sxs-lookup"><span data-stu-id="58352-110">Click **Search**.</span></span>

<span data-ttu-id="58352-111">في النتائج، انقر فوق **عامل تصفية النتائج** واكتب **علبة مجموعة** في المربع النشاط.</span><span class="sxs-lookup"><span data-stu-id="58352-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="58352-112">حدد سجل تدقيق في النتائج.</span><span class="sxs-lookup"><span data-stu-id="58352-112">Select an audit record in the results.</span></span> <span data-ttu-id="58352-113">في القائمة الفرعية **تفاصيل** ، انقر فوق **مزيد من المعلومات**.</span><span class="sxs-lookup"><span data-stu-id="58352-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="58352-114">يجب عليك مراجعة تفاصيل كل سجل التدوين لتحديد حالة تتعلق بالنشاط إرسال البريد الإلكتروني.</span><span class="sxs-lookup"><span data-stu-id="58352-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="58352-115">**ObjectId**: قيمة الاسم المستعار علبة البريد التي تم تعديلها.</span><span class="sxs-lookup"><span data-stu-id="58352-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="58352-116">**المعلمات**: _فورواردينجسمتبادريس_ يشير إلى عنوان البريد الإلكتروني الهدف.</span><span class="sxs-lookup"><span data-stu-id="58352-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="58352-117">**اسم المستخدم**: المستخدم الذي قام بتكوين إعادة توجيه البريد الإلكتروني في صندوق البريد في ميدان **ObjectId** .</span><span class="sxs-lookup"><span data-stu-id="58352-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="58352-118">لمزيد من المعلومات، راجع [تحديد الذي قام بإعداد علبة بريد إرسال البريد الإلكتروني](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="58352-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
