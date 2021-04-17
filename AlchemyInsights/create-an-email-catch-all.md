---
title: إنشاء التقاط للبريد الإلكتروني الكل
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816187"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="6fc8a-102">إنشاء التقاط للبريد الإلكتروني الكل</span><span class="sxs-lookup"><span data-stu-id="6fc8a-102">Create an email catch all</span></span>

<span data-ttu-id="6fc8a-103">لا يشجع استخدام المصيد على الإطلاق بشدة.</span><span class="sxs-lookup"><span data-stu-id="6fc8a-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="6fc8a-104">من الأفضل توفير ارتداد إلى المرسل للسماح للمرسلين بعلم أنه لا يمكن تسليم رسالتهم كمعالجة حتى يمكنهم اتخاذ إجراء ما.</span><span class="sxs-lookup"><span data-stu-id="6fc8a-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="6fc8a-105">يمكنك أيضا تقييد علبة البريد التي تم مراقبتها لالتقاط عناوين البريد الإلكتروني الصالحة سابقا فقط.</span><span class="sxs-lookup"><span data-stu-id="6fc8a-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="6fc8a-106">ستتلقى أي علبة بريد ملتقطة الكثير من البريد العشوائي وقد تملأها في النهاية إذا لم يتم مراقبتها عن كثب.</span><span class="sxs-lookup"><span data-stu-id="6fc8a-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="6fc8a-107">(هناك حدود مستلمة.)</span><span class="sxs-lookup"><span data-stu-id="6fc8a-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="6fc8a-108">إذا قررت المتابعة، فاتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="6fc8a-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="6fc8a-109">إنشاء مجموعة توزيع ديناميكية & تتضمن "كافة أنواع المستلمين".</span><span class="sxs-lookup"><span data-stu-id="6fc8a-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="6fc8a-110">أنشئ علبة بريد مخصصة لالتقاط رسائل البريد الإلكتروني، على سبيل المثال، catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="6fc8a-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="6fc8a-111">بالنسبة للمجال المحدد، قم بتعيين DomainType إلى "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="6fc8a-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="6fc8a-112">إذا قمت لاحقا بإزالة التقاط الكل، فتأكد من تعيين المجال مرة أخرى إلى موثوق.</span><span class="sxs-lookup"><span data-stu-id="6fc8a-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="6fc8a-113">إنشاء قاعدة نقل تدفق البريد كما يلي:</span><span class="sxs-lookup"><span data-stu-id="6fc8a-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="6fc8a-114">إذا كان المرسل "خارج المؤسسة"</span><span class="sxs-lookup"><span data-stu-id="6fc8a-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="6fc8a-115">إعادة توجيه الرسالة إلى Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="6fc8a-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="6fc8a-116">باستثناء ما إذا كان المستلم عضوا في allusers@domain.com (تحتوي مجموعة التوزيع على كل الأعضاء)</span><span class="sxs-lookup"><span data-stu-id="6fc8a-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="6fc8a-117">التأكد من صحة إضافة علب بريد جديدة إلى مجموعة التوزيع الديناميكي</span><span class="sxs-lookup"><span data-stu-id="6fc8a-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
