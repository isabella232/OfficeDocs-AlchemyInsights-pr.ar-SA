---
title: إنشاء رسالة بريد الكتروني للتقاط الكل
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712973"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="ba90c-102">إنشاء رسالة بريد الكتروني للتقاط الكل</span><span class="sxs-lookup"><span data-stu-id="ba90c-102">Create an email catch all</span></span>

<span data-ttu-id="ba90c-103">استخدام الأمر "التقاط الكل" ديسكوراجيد بشده.</span><span class="sxs-lookup"><span data-stu-id="ba90c-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="ba90c-104">من الأفضل توفير ارتداد إلى المرسل لتمكين المرسلين من التعرف علي الرسائل الخاصة بهم لكي يتمكنوا من القيام بالإجراءات.</span><span class="sxs-lookup"><span data-stu-id="ba90c-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="ba90c-105">يمكنك أيضا تحديد علبه البريد المراقبة للتقاط عناوين البريد الكتروني الصالحة مسبقا فقط.</span><span class="sxs-lookup"><span data-stu-id="ba90c-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="ba90c-106">ستتلقى إيه علبه بريد بالبالكامل الكل طريقه جيده من البريد العشوائي وقد تملا في النهاية إذا لم يتم الاطلاع عليها بشكل كامل.</span><span class="sxs-lookup"><span data-stu-id="ba90c-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="ba90c-107">(هناك حدود التلقي.)</span><span class="sxs-lookup"><span data-stu-id="ba90c-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="ba90c-108">إذا قررت المتابعة ، فاتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="ba90c-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="ba90c-109">إنشاء مجموعه توزيع ديناميكية & تتضمن "كل أنواع المستلمين".</span><span class="sxs-lookup"><span data-stu-id="ba90c-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="ba90c-110">إنشاء علبه بريد مخصصه للتقاط رسائل البريد الكتروني ، علي سبيل المثال ، catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="ba90c-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="ba90c-111">بالنسبة للمجال المحدد ، قم بتعيين دوماينتيبي إلى "إينتيرنالريلاي".</span><span class="sxs-lookup"><span data-stu-id="ba90c-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="ba90c-112">إذا قمت بازاله الكل لاحقا ، فتاكد من أعاده تعيين المجال إلى مخول.</span><span class="sxs-lookup"><span data-stu-id="ba90c-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="ba90c-113">قم بإنشاء قاعده نقل بحث https://configure.office.com/scenario.aspx?sid=12 علي النحو التالي:</span><span class="sxs-lookup"><span data-stu-id="ba90c-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="ba90c-114">إذا كان المرسل هو "خارج المؤسسة"</span><span class="sxs-lookup"><span data-stu-id="ba90c-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="ba90c-115">أعاده توجيه الرسالة إلى Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="ba90c-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="ba90c-116">ما لم يكن المستلم عضوا في allusers@domain.com (تحتوي مجموعه التوزيع علي كل الأعضاء)</span><span class="sxs-lookup"><span data-stu-id="ba90c-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="ba90c-117">التاكد من التحقق من أضافه علب البريد الجديدة إلى مجموعه التوزيع الديناميكية</span><span class="sxs-lookup"><span data-stu-id="ba90c-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
