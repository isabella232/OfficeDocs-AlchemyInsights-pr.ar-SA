---
title: 1332 OWA-قواعد علبة الوارد لا تنفذ لعلبة بريد
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 0d3b7ce3d6b32d94a012eb3767c0747eed80f6e5
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29915791"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="6efb2-102">قاعدة الوارد لا يعمل كما هو متوقع</span><span class="sxs-lookup"><span data-stu-id="6efb2-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="6efb2-103">تحقق من الإعدادات التالية:</span><span class="sxs-lookup"><span data-stu-id="6efb2-103">Verify the following settings:</span></span>
  
- <span data-ttu-id="6efb2-p101">يمكن إعادة توجيه رسالة، التي تم إعادة توجيهها أو الرد عليها تلقائياً استناداً إلى قواعد علبة الوارد مرة واحدة فقط. إضافة قاعدة إعادة توجيه (قاعدة علبة الوارد أو قاعدة تدفق البريد، تعرف أيضا باسم قاعدة نقل) كحد أقصى عشرة المستلمين إعادة التوجيه إلى رسالة. لمزيد من المعلومات، راجع [حدود قواعد دفتر اليومية، والنقل، وعلبة الوارد](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="6efb2-p101">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time. A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message. For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>
    
- <span data-ttu-id="6efb2-p102">لا تعمل قواعد علبة الوارد على علبة البريد اليومية بديلة. لمزيد من المعلومات حول البديل اليومية علبة البريد، راجع [علبة البريد اليومية بديلة](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="6efb2-p102">Inbox rules don't work on the alternate journaling mailbox. For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>
    
<span data-ttu-id="6efb2-109">لحل هذه المشكلات، راجع [2829319 كيلو بايت](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="6efb2-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>
  
<span data-ttu-id="6efb2-110">إذا لم تقم بتطبيق الإعداد السابقة، تشغيل تقرير التشخيص قاعدة الوارد قبل أن يمكنك تصعيد المشكلة إلى "دعم microsoft":</span><span class="sxs-lookup"><span data-stu-id="6efb2-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>
  
1. <span data-ttu-id="6efb2-111">فتح علبة البريد في Outlook على الويب، وانقر فوق **إعدادات** \> **خيارات** \> **تنظيم البريد الإلكتروني** \> **قواعد علبة الوارد**.</span><span class="sxs-lookup"><span data-stu-id="6efb2-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>
    
2. <span data-ttu-id="6efb2-112">في أسفل الصفحة، انقر فوق **حالة القواعد لا تعمل انقر هنا لإنشاء تقرير تشخيص**.</span><span class="sxs-lookup"><span data-stu-id="6efb2-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
    

