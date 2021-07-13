---
title: تجمع الترحيل الصادر
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/08/2021
ms.locfileid: "53381561"
---
# <a name="outbound-relay-pool"></a><span data-ttu-id="cbeeb-102">تجمع الترحيل الصادر</span><span class="sxs-lookup"><span data-stu-id="cbeeb-102">Outbound relay pool</span></span>

<span data-ttu-id="cbeeb-103">تقوم Microsoft بإجراء بعض التغييرات على التكوين لترحيل البريد الإلكتروني أو إعادة توجيهه عبر Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="cbeeb-103">Microsoft is making some changes to the configuration for relaying or forwarding email through Microsoft 365.</span></span> <span data-ttu-id="cbeeb-104">يتم إعادة توجيه الرسائل في سيناريوهات معينة أو ترحيلها Microsoft 365 باستخدام تجمع ترحيل خاص.</span><span class="sxs-lookup"><span data-stu-id="cbeeb-104">Messages in certain scenarios are forwarded or relayed through Microsoft 365 using a special relay pool.</span></span> <span data-ttu-id="cbeeb-105">قد تنتهي الرسائل المرسلة باستخدام تجمع الترحيل في مجلد البريد غير الهام الخاص بالمستلم.</span><span class="sxs-lookup"><span data-stu-id="cbeeb-105">Messages sent by using the relay pool could end up in recipient's junk mail folder.</span></span> <span data-ttu-id="cbeeb-106">لمزيد من المعلومات، راجع [تجمعات التسليم الصادرة](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span><span class="sxs-lookup"><span data-stu-id="cbeeb-106">For more information, see [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span></span>

<span data-ttu-id="cbeeb-107">لتجنب سيناريو باستخدام تجمع الترحيل، تأكد من أن الرسائل التي تم إعادة توجيهها/ترحيلها تلبي أحد المعايير التالية:</span><span class="sxs-lookup"><span data-stu-id="cbeeb-107">To avoid a scenario using the relay pool, make sure that forwarded/relayed messages meet one of the following criteria:</span></span>

- <span data-ttu-id="cbeeb-108">المرسل الصادر هو مجال مقبول للمستأجر.</span><span class="sxs-lookup"><span data-stu-id="cbeeb-108">The outbound sender is an accepted domain of the tenant.</span></span>
- <span data-ttu-id="cbeeb-109">يمر إطار نهج المرسل (SPF) عندما تظهر الرسالة Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="cbeeb-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span></span>
- <span data-ttu-id="cbeeb-110">يتم تمرير DomainKeys Identified Mail (DKIM) على مجال مرسل P2 عندما تظهر الرسالة Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="cbeeb-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span></span>
 
<span data-ttu-id="cbeeb-111">لا يتم ترحيل الرسائل التي تفي بالمعايير أعلاه عبر تجمع الترحيل.</span><span class="sxs-lookup"><span data-stu-id="cbeeb-111">Messages that meet the above criteria are not relayed through the relay pool.</span></span>

<span data-ttu-id="cbeeb-112">إذا كان سجل MX لمجالك مشارا إلى خادم جهة خارجية أو خادم داخلي، فاستخدم التصفية المحسنة للتأكد من صحة التحقق من صحة SPF للبريد الإلكتروني الوارد ولتجنب إرسال البريد الإلكتروني عبر تجمع الترحيل.</span><span class="sxs-lookup"><span data-stu-id="cbeeb-112">If the MX record for your domain is pointed to a third-party or on-premises server, use enhanced filtering to make sure the SPF validation is correct for inbound email and to avoid sending email through the relay pool.</span></span>

<span data-ttu-id="cbeeb-113">**كيف يمكننا معرفة ما إذا كان تجمع الترحيل متأثيا؟**</span><span class="sxs-lookup"><span data-stu-id="cbeeb-113">**How can we tell if we're impacted by the relay pool?**</span></span>

<span data-ttu-id="cbeeb-114">إذا كانت رسائل البريد الإلكتروني التي تم إعادة توجيهها أو ترحيلها تستخدم أحد المعايير أعلاه، فلن يتم ترحيل الرسائل عبر تجمع الترحيل.</span><span class="sxs-lookup"><span data-stu-id="cbeeb-114">If your forwarded or relayed emails use one of the above criteria, messages won't be relayed through the relay pool.</span></span> <span data-ttu-id="cbeeb-115">ومع ذلك، إذا تم إرسال رسالة عبر تجمع ترحيل، فإن IP للخادم الصادر يكون في النطاق 40.95.0.0/16 ويتضمن اسم الخادم الصادر **rly** في الاسم.</span><span class="sxs-lookup"><span data-stu-id="cbeeb-115">However, if a message is sent through a relay pool, the outbound server IP is in the 40.95.0.0/16 range and the outbound server name includes **rly** in the name.</span></span>

