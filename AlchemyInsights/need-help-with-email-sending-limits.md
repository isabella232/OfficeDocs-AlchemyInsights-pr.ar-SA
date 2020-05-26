---
title: هل تحتاج إلى مساعدة في إرسال حدود البريد الإلكتروني؟
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 7f563df313c869d18c3e4240d271c649a74914af
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357258"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="bed03-102">هل تحتاج إلى مساعدة في إرسال حدود البريد الإلكتروني؟</span><span class="sxs-lookup"><span data-stu-id="bed03-102">Need help with email sending limits?</span></span>

<span data-ttu-id="bed03-103">وفيما يلي **حدود الإرسال حسب التصميم** المفروضة في الخدمة.</span><span class="sxs-lookup"><span data-stu-id="bed03-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="bed03-104">يتم توثيق مزيد من المعلومات حول هذه الحدود [هنا](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="bed03-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="bed03-105">لتثبيط تسليم الرسائل المجمعة غير المرغوب فيها، نقوم بتطبيق حدود معدل المستلم لكل مستخدم **على كافة الرسائل الصادرة والداخلية.**</span><span class="sxs-lookup"><span data-stu-id="bed03-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="bed03-106">في جميع SKUs، هذا الحد هو **10،000 المتلقين يوميا.**</span><span class="sxs-lookup"><span data-stu-id="bed03-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="bed03-107">يجب على العملاء الذين يحتاجون إلى إرسال بريد إلكتروني تجاري مجمع شرعي (على سبيل المثال، الرسائل الإخبارية للعملاء) استخدام موفري جهات خارجية متخصصين في هذه الخدمات.</span><span class="sxs-lookup"><span data-stu-id="bed03-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="bed03-108">**ملاحظة:** بمجرد الوصول إلى حد معدل المستلمين، لا يمكن إرسال الرسائل من صندوق البريد حتى ينخفض عدد المستلمين الذين تم إرسال رسائل في الـ 24 ساعة الماضية إلى أقل من الحد.</span><span class="sxs-lookup"><span data-stu-id="bed03-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="bed03-109">لن يتمكن المستخدم من إرسال رسائل حتى تلك النقطة.</span><span class="sxs-lookup"><span data-stu-id="bed03-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="bed03-110">يتم تطبيق حد معدل الرسائل **30 رسالة في الدقيقة عبر** كافة SKUs.</span><span class="sxs-lookup"><span data-stu-id="bed03-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="bed03-111">يحدد هذا عدد الرسائل التي يمكن للمستخدم إرسالها من حسابه Exchange Online خلال فترة محددة.</span><span class="sxs-lookup"><span data-stu-id="bed03-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="bed03-112">**الحد الأقصى لعدد المستلمين المسموح به في** حقول To و Cc و Bcc لرسالة بريد إلكتروني واحدة، عبر جميع SKUs، هو **1000 مستلم**.</span><span class="sxs-lookup"><span data-stu-id="bed03-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="bed03-113">لتخصيص هذا الحد، انتقل [هنا](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="bed03-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
