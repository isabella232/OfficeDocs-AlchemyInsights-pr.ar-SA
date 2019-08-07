---
title: 1332 OWA-قواعد علبة الوارد لا تنفذ لعلبة بريد
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 218a05a8d321b76dd07345ea48d6b3e158cc120e
ms.sourcegitcommit: 77f704672b7c7de541899e25c022ff10c111e304
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2019
ms.locfileid: "36204047"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="18863-102">قاعدة الوارد لا يعمل كما هو متوقع</span><span class="sxs-lookup"><span data-stu-id="18863-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="18863-103">تحقق من الإعدادات التالية:</span><span class="sxs-lookup"><span data-stu-id="18863-103">Verify the following settings:</span></span>

- <span data-ttu-id="18863-104">يمكن إعادة توجيه رسالة، التي تم إعادة توجيهها أو الرد عليها تلقائياً استناداً إلى قواعد علبة الوارد مرة واحدة فقط.</span><span class="sxs-lookup"><span data-stu-id="18863-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="18863-105">إضافة قاعدة إعادة توجيه (قاعدة علبة الوارد أو قاعدة تدفق البريد، تعرف أيضا باسم قاعدة نقل) كحد أقصى عشرة المستلمين إعادة التوجيه إلى رسالة.</span><span class="sxs-lookup"><span data-stu-id="18863-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="18863-106">لمزيد من المعلومات، راجع [حدود قواعد دفتر اليومية، والنقل، وعلبة الوارد](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="18863-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="18863-107">لا تعمل قواعد علبة الوارد على علبة البريد اليومية بديلة.</span><span class="sxs-lookup"><span data-stu-id="18863-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="18863-108">لمزيد من المعلومات حول البديل اليومية علبة البريد، راجع [علبة البريد اليومية بديلة](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="18863-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="18863-109">لحل هذه المشكلات، راجع [2829319 كيلو بايت](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="18863-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="18863-110">إذا لم تقم بتطبيق الإعداد السابقة، تشغيل تقرير التشخيص قاعدة الوارد قبل أن يمكنك تصعيد المشكلة إلى "دعم microsoft":</span><span class="sxs-lookup"><span data-stu-id="18863-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="18863-111">فتح علبة البريد في Outlook على الويب وانقر فوق</span><span class="sxs-lookup"><span data-stu-id="18863-111">Open the mailbox in Outlook on the web, and click</span></span> <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 <span data-ttu-id="18863-112">**إعدادات** > **عرض كافة إعدادات Outlook** > **البريد** > **القواعد**.</span><span class="sxs-lookup"><span data-stu-id="18863-112">**Settings** > **View all Outlook Settings** > **Mail** > **Rules**.</span></span>

2. <span data-ttu-id="18863-113">في أسفل الصفحة، انقر فوق **حالة القواعد لا تعمل انقر هنا لإنشاء تقرير تشخيص**.</span><span class="sxs-lookup"><span data-stu-id="18863-113">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
