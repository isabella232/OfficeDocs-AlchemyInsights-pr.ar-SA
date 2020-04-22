---
title: تحديد إعادة توجيه البريد الإلكتروني الخارجي على صناديق البريد في سجلات التدقيق
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 156fd0044cdc42230ace0a5db16f49af572bb6fa
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716447"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="c64ee-102">تحديد وقت تكوين إعادة توجيه البريد الإلكتروني الخارجي على صناديق البريد</span><span class="sxs-lookup"><span data-stu-id="c64ee-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="c64ee-103">عندما يقوم مستخدم Microsoft 365 بتكوين إعادة توجيه البريد الإلكتروني الخارجي على علبة بريد، يتم تدقيق النشاط كجزء من **cmdlet Set-علبة البريد.**</span><span class="sxs-lookup"><span data-stu-id="c64ee-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="c64ee-104">يمكنك مشاهدة النشاط باستخدام بحث سجل التدقيق في مركز التوافق & الأمان.</span><span class="sxs-lookup"><span data-stu-id="c64ee-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="c64ee-105">تسجيل الدخول إلى [مركز التوافق & الأمان Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="c64ee-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="c64ee-106">انتقل إلى صفحة البحث في**سجل تدقيق** **البحث.** > </span><span class="sxs-lookup"><span data-stu-id="c64ee-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="c64ee-107">حدد نطاق التاريخ في **حقول تاريخ البدء** وتاريخ **الانتهاء.**</span><span class="sxs-lookup"><span data-stu-id="c64ee-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="c64ee-108">لا تحتاج إلى تحديد اسم مستخدم.</span><span class="sxs-lookup"><span data-stu-id="c64ee-108">You don't need to specify a username.</span></span> <span data-ttu-id="c64ee-109">تحقق من تعيين حقل **الأنشطة** **لإظهار النتائج لكافة الأنشطة**.</span><span class="sxs-lookup"><span data-stu-id="c64ee-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="c64ee-110">انقر فوق **البحث**.</span><span class="sxs-lookup"><span data-stu-id="c64ee-110">Click **Search**.</span></span>

<span data-ttu-id="c64ee-111">في النتائج، انقر فوق **نتائج التصفية** واكتب **تعيين علبة البريد** في مربع عامل تصفية النشاط.</span><span class="sxs-lookup"><span data-stu-id="c64ee-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="c64ee-112">حدد سجل تدقيق في النتائج.</span><span class="sxs-lookup"><span data-stu-id="c64ee-112">Select an audit record in the results.</span></span> <span data-ttu-id="c64ee-113">في **التفاصيل** المنبثقة، انقر فوق **مزيد من المعلومات**.</span><span class="sxs-lookup"><span data-stu-id="c64ee-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="c64ee-114">يجب عليك الاطلاع على تفاصيل كل سجل تدقيق لتحديد ما إذا كان النشاط مرتبطًا بإعادة توجيه البريد الإلكتروني.</span><span class="sxs-lookup"><span data-stu-id="c64ee-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="c64ee-115">**ObjectId:** قيمة الاسم المستعار لصندوق البريد الذي تم تعديله.</span><span class="sxs-lookup"><span data-stu-id="c64ee-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="c64ee-116">**المعلمات**: _يشير إعادة توجيه SmtpAddress_ إلى عنوان البريد الإلكتروني المستهدف.</span><span class="sxs-lookup"><span data-stu-id="c64ee-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="c64ee-117">**معرف المستخدم:** المستخدم الذي قام بتكوين إعادة توجيه البريد الإلكتروني على علبة البريد في حقل **ObjectId.**</span><span class="sxs-lookup"><span data-stu-id="c64ee-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="c64ee-118">لمزيد من المعلومات، راجع [تحديد من قام بإعداد إعادة توجيه البريد الإلكتروني لعلبة بريد](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="c64ee-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
