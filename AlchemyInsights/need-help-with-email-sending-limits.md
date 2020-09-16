---
title: هل تحتاج إلى المساعدة بشان حدود إرسال البريد الكتروني ؟
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 66ff82afd7b44ef5fd4943bfc794c2fa35bbfa9e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702350"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="b516c-102">هل تحتاج إلى المساعدة بشان حدود إرسال البريد الكتروني ؟</span><span class="sxs-lookup"><span data-stu-id="b516c-102">Need help with email sending limits?</span></span>

<span data-ttu-id="b516c-103">فيما يلي أدناه **قيود الإرسال** التي يتم فرضها في الخدمة.</span><span class="sxs-lookup"><span data-stu-id="b516c-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="b516c-104">المزيد من المعلومات حول هذه الحدود موثقه [هنا](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="b516c-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="b516c-105">لحظر تسليم الرسائل غير المرغوب فيها ، قمنا بتطبيق **حدود معدل المستلمين لكل مستخدم علي كل الرسائل الصادرة والداخلية**.</span><span class="sxs-lookup"><span data-stu-id="b516c-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="b516c-106">عبر كل وحدات Sku ، يكون هذا الحد هو **10,000 مستلما في اليوم**.</span><span class="sxs-lookup"><span data-stu-id="b516c-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="b516c-107">يجب علي العملاء الذين يحتاجون إلى إرسال رسائل بريد الكتروني تجاريه مجمعه (علي سبيل المثال ، رسائل إخباريه للعملاء) استخدام موفري الجهات الخارجية المتخصصين في هذه الخدمات.</span><span class="sxs-lookup"><span data-stu-id="b516c-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="b516c-108">**ملاحظه**: بمجرد الوصول إلى الحد الأقصى لمعدل الإرسال ، لا يمكن إرسال الرسائل من علبه البريد إلى ان يتجاوز عدد المستلمين الذين أرسلوا رسائل في الساعات الماضية والتي تم إرسالها إلى اقل من الحد.</span><span class="sxs-lookup"><span data-stu-id="b516c-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="b516c-109">لن يتمكن المستخدم من إرسال الرسائل حتى تلك النقطة.</span><span class="sxs-lookup"><span data-stu-id="b516c-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="b516c-110">يتم تطبيق حد سرعه الرسالة الذي يبلغ **30 رسالة لكل دقيقه** عبر كل وحدات sku.</span><span class="sxs-lookup"><span data-stu-id="b516c-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="b516c-111">يحدد هذا الاجراء عدد الرسائل التي يستطيع المستخدم إرسالها من حساب Exchange Online الخاص بها خلال فتره زمنيه محدده.</span><span class="sxs-lookup"><span data-stu-id="b516c-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="b516c-112">**الحد الأقصى لعدد المستلمين المسموح بهم في الحقول "إلى" و "نسخه" و "مخفيه** " لرسالة بريد الكتروني واحده ، عبر كل وحدات sku ، هو **1000 مستلما**.</span><span class="sxs-lookup"><span data-stu-id="b516c-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="b516c-113">لتخصيص هذا الحد ، انتقل إلى [هنا](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="b516c-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
