---
title: 1332 OWA-قاعده (قواعد) علبه الوارد لا يتم تنفيذها لعلبه بريد
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: f4d8db9c590abc490f193ef54a8a1dc5afba82b9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721578"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="0cf77-102">لا تعمل قاعده علبه الوارد كما هو متوقع</span><span class="sxs-lookup"><span data-stu-id="0cf77-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="0cf77-103">تحقق من الإعدادات التالية في Outlook علي الويب:</span><span class="sxs-lookup"><span data-stu-id="0cf77-103">Verify the following settings in Outlook on the web:</span></span>

- <span data-ttu-id="0cf77-104">يمكن أعاده توجيه رسالة أو أعاده توجيهها أو الرد عليها تلقائيا استنادا إلى قواعد علبه الوارد مره واحده فقط.</span><span class="sxs-lookup"><span data-stu-id="0cf77-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="0cf77-105">يمكن لقاعده أعاده التوجيه (قاعده علبه الوارد أو قاعده البريد الكتروني ، المعروفة أيضا بقاعده النقل) أضافه عشره مستلمين بحد اقصي إلى الرسالة.</span><span class="sxs-lookup"><span data-stu-id="0cf77-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="0cf77-106">لمزيد من المعلومات ، راجع [حدود قواعد اليومية والنقل وعلبه الوارد](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="0cf77-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="0cf77-107">لا تعمل قواعد علبه الوارد علي علبه بريد اليومية البديلة.</span><span class="sxs-lookup"><span data-stu-id="0cf77-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="0cf77-108">للحصول علي مزيد من المعلومات حول علبه بريد اليومية البديلة ، راجع [علبه بريد اليومية البديلة](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="0cf77-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="0cf77-109">لإصلاح هذه المشاكل ، راجع [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="0cf77-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="0cf77-110">إذا لم يتم تطبيق المشاكل السابقة ، فقم بتشغيل تقرير تشخيص قاعده علبه الوارد قبل ان تقوم بتصعيد المشكلة إلى دعم Microsoft:</span><span class="sxs-lookup"><span data-stu-id="0cf77-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="0cf77-111">افتح علبه البريد في Outlook علي الويب ، وانقر فوق</span><span class="sxs-lookup"><span data-stu-id="0cf77-111">Open the mailbox in Outlook on the web, and click</span></span> <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 <span data-ttu-id="0cf77-112">**إعدادات**  >  **عرض كل إعدادات Outlook**  >  **البريد**  >  **قواعد**.</span><span class="sxs-lookup"><span data-stu-id="0cf77-112">**Settings** > **View all Outlook Settings** > **Mail** > **Rules**.</span></span>

2. <span data-ttu-id="0cf77-113">في أسفل الصفحة ، انقر فوق **إذا كانت القواعد لا تعمل ، فانقر هنا لإنشاء تقرير تشخيصي**.</span><span class="sxs-lookup"><span data-stu-id="0cf77-113">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
