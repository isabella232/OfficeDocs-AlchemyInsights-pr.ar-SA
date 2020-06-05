---
title: 1332 OWA - قاعدة علبة الوارد (قواعد) لا يتم تنفيذها لصندوق بريد
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 9abdcdcb33d39b8b9fe2df80f0c15a8b55e465fd
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/05/2020
ms.locfileid: "44576547"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="7614c-102">لا تعمل قاعدة علبة الوارد كما هو متوقع</span><span class="sxs-lookup"><span data-stu-id="7614c-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="7614c-103">تحقق من الإعدادات التالية في Outlook على الويب:</span><span class="sxs-lookup"><span data-stu-id="7614c-103">Verify the following settings in Outlook on the web:</span></span>

- <span data-ttu-id="7614c-104">يمكن إعادة توجيه الرسالة أو إعادة توجيهها أو الرد عليها تلقائيًا استنادًا إلى قواعد علبة الوارد مرة واحدة فقط.</span><span class="sxs-lookup"><span data-stu-id="7614c-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="7614c-105">يمكن لقاعدة إعادة التوجيه (قاعدة علبة الوارد أو قاعدة تدفق البريد، المعروفة أيضًا باسم قاعدة النقل) إضافة عشرة مستلمين لإعادة التوجيه كحد أقصى إلى رسالة.</span><span class="sxs-lookup"><span data-stu-id="7614c-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="7614c-106">لمزيد من المعلومات، راجع [حدود قاعدة دفتر اليومية والنقل وعلبة الوارد](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="7614c-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="7614c-107">لا تعمل قواعد علبة الوارد على علبة البريد اليومية البديلة.</span><span class="sxs-lookup"><span data-stu-id="7614c-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="7614c-108">لمزيد من المعلومات حول علبة البريد دفتر اليومية البديلة، راجع [علبة بريد دفتر اليومية البديلة](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="7614c-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="7614c-109">لإصلاح هذه المشكلات، راجع [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="7614c-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="7614c-110">في حالة عدم تطبيق المشكلات السابقة، قم بتشغيل تقرير تشخيص قاعدة علبة الوارد قبل تصعيد المشكلة إلى دعم Microsoft:</span><span class="sxs-lookup"><span data-stu-id="7614c-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="7614c-111">فتح علبة البريد في Outlook على الويب، وانقر فوق</span><span class="sxs-lookup"><span data-stu-id="7614c-111">Open the mailbox in Outlook on the web, and click</span></span> <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 <span data-ttu-id="7614c-112">**الإعدادات**  >  **عرض كافة إعدادات**  >  Outlook **البريد**  >  **القواعد**.</span><span class="sxs-lookup"><span data-stu-id="7614c-112">**Settings** > **View all Outlook Settings** > **Mail** > **Rules**.</span></span>

2. <span data-ttu-id="7614c-113">في أسفل الصفحة، انقر فوق **إذا كانت القواعد لا تعمل انقر هنا لإنشاء تقرير تشخيصي**.</span><span class="sxs-lookup"><span data-stu-id="7614c-113">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
