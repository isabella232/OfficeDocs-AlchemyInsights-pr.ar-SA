---
title: إنشاء رسالة بريد إلكتروني التقاط الكل
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286019"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="399df-102">إنشاء رسالة بريد إلكتروني التقاط الكل</span><span class="sxs-lookup"><span data-stu-id="399df-102">Create an email catch all</span></span>

<span data-ttu-id="399df-103">يتم تثبيط استخدام الصيد كل شيء بقوة.</span><span class="sxs-lookup"><span data-stu-id="399df-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="399df-104">من الأفضل توفير ارتداد إلى المرسل لإعلام المرسلين بأنه لا يمكن تسليم رسالتهم كما تم توجيهها حتى يتمكنوا من اتخاذ إجراء.</span><span class="sxs-lookup"><span data-stu-id="399df-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="399df-105">يمكنك أيضًا تحديد علبة البريد المراقبة لالتقاط عناوين البريد الإلكتروني الصالحة سابقًا فقط.</span><span class="sxs-lookup"><span data-stu-id="399df-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="399df-106">أي التقاط جميع علبة البريد سوف تتلقى قدرا كبيرا من البريد المزعج ، وربما في نهاية المطاف ملء إذا لم يتم رصدها عن كثب.</span><span class="sxs-lookup"><span data-stu-id="399df-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="399df-107">(هناك حدود تلقي.)</span><span class="sxs-lookup"><span data-stu-id="399df-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="399df-108">إذا قررت المتابعة، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="399df-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="399df-109">إنشاء مجموعة توزيع ديناميكية & تتضمن "كافة أنواع المستلمين".</span><span class="sxs-lookup"><span data-stu-id="399df-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="399df-110">إنشاء علبة بريد مخصصة لالتقاط رسائل البريد الإلكتروني، على سبيل المثال، catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="399df-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="399df-111">للمجال المحدد، قم بتعيين DomainType إلى "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="399df-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="399df-112">إذا قمت لاحقاً بإزالة الكل، تأكد من تعيين المجال مرة أخرى إلى موثوقبه.</span><span class="sxs-lookup"><span data-stu-id="399df-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="399df-113">إنشاء قاعدة نقل تدفق البريد على النحو التالي:</span><span class="sxs-lookup"><span data-stu-id="399df-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="399df-114">إذا كان المرسل "خارج المؤسسة"</span><span class="sxs-lookup"><span data-stu-id="399df-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="399df-115">إعادة توجيه الرسالة إلى Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="399df-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="399df-116">إلا إذا كان المستلم عضواً في allusers@domain.com (مجموعة التوزيع تحتوي على كافة الأعضاء)</span><span class="sxs-lookup"><span data-stu-id="399df-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="399df-117">التأكد من صحة إضافة علب البريد الجديدة إلى مجموعة التوزيع الديناميكي</span><span class="sxs-lookup"><span data-stu-id="399df-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
