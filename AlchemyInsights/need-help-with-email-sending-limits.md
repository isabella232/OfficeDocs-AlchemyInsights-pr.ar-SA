---
title: هل تحتاج إلى مساعدة في تحديد حدود إرسال البريد الإلكتروني؟
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: b5bdfbf818328c97ec93b3468aeedcbe88e03913
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836266"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="3f469-102">هل تحتاج إلى مساعدة في تحديد حدود إرسال البريد الإلكتروني؟</span><span class="sxs-lookup"><span data-stu-id="3f469-102">Need help with email sending limits?</span></span>

<span data-ttu-id="3f469-103">فيما يلي **حدود الإرسال حسب التصميم المفروضة** في الخدمة.</span><span class="sxs-lookup"><span data-stu-id="3f469-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="3f469-104">يتم توثيق مزيد من المعلومات حول هذه الحدود [هنا](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="3f469-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="3f469-105">لتثبيط تسليم الرسائل المجمعة غير المرغوب فيها، نطبق قيود أسعار المستلمين لكل مستخدم على كل الرسائل الصادرة **والداخلية.**</span><span class="sxs-lookup"><span data-stu-id="3f469-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="3f469-106">في كل SKUs، هذا الحد هو **10000** مستلم في اليوم .</span><span class="sxs-lookup"><span data-stu-id="3f469-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="3f469-107">يجب على العملاء الذين يحتاجون إلى إرسال بريد إلكتروني تجاري مجمع شرعي (على سبيل المثال، رسائل العملاء الإخبارية) استخدام موفرين من جهة خارجية متخصصين في هذه الخدمات.</span><span class="sxs-lookup"><span data-stu-id="3f469-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="3f469-108">**ملاحظة:** بمجرد الوصول إلى حد سعر المستلم، لا يمكن إرسال الرسائل من علبة البريد حتى ينخفض عدد المستلمين الذين تم إرسال الرسائل خلال ال 24 ساعة الماضية إلى أقل من الحد.</span><span class="sxs-lookup"><span data-stu-id="3f469-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="3f469-109">لن يتمكن المستخدم من إرسال الرسائل حتى تلك النقطة.</span><span class="sxs-lookup"><span data-stu-id="3f469-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="3f469-110">يتم تطبيق حد معدل **الرسائل وهو 30 رسالة في** الدقيقة عبر كل SKUs.</span><span class="sxs-lookup"><span data-stu-id="3f469-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="3f469-111">يحدد ذلك عدد الرسائل التي يمكن للمستخدم إرسالها من حساب Exchange Online الخاص به خلال فترة زمنية محددة.</span><span class="sxs-lookup"><span data-stu-id="3f469-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="3f469-112">إن **الحد الأقصى لعدد** المستلمين المسموح به في الحقول "إلى" و"نسخة" و"نسخة"، و"نسخة"، لرسالة بريد إلكتروني واحدة، عبر كل "وحدة SKUs"، هو **1000** مستلم.</span><span class="sxs-lookup"><span data-stu-id="3f469-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="3f469-113">لتخصيص هذا الحد، انتقل [إلى هنا](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="3f469-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
