---
title: استدعاء رسالة بريد الكتروني أو استبدالها
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 2e711679e7db7293d9e7e6f68d0662f03047c23d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799191"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="50058-102">استدعاء رسالة بريد الكتروني أو استبدالها في Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="50058-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="50058-103">يمكنك **فقط استدعاء الرسائل التي يتم إرسالها إلى الأشخاص في مؤسستك**.</span><span class="sxs-lookup"><span data-stu-id="50058-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="50058-104">إذا تم إرسال الرسالة إلى عنوان Gmail ، علي سبيل المثال ، لا يمكنك استدعاؤها.</span><span class="sxs-lookup"><span data-stu-id="50058-104">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="50058-105">يمكنك **فقط استدعاء الرسائل المرسلة من Outlook 2016 للكمبيوتر الشخصي**.</span><span class="sxs-lookup"><span data-stu-id="50058-105">You can **only recall messages sent from Outlook 2016 for the PC**.</span></span> <span data-ttu-id="50058-106">إذا أرسل أحد المستخدمين رسالة باستخدام Outlook for Mac أو Outlook علي الويب ، فلا يمكنك استدعاؤه.</span><span class="sxs-lookup"><span data-stu-id="50058-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="50058-107">إذا كنت مسؤولا ، فيمكنك **استدعاء الرسائل بالنيابة عن المستخدمين باستخدام PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="50058-107">If you're an admin, you can **recall messages on behalf of users by using PowerShell**.</span></span> <span data-ttu-id="50058-108">لا يمكنك استدعاء الرسائل من مركز الاداره.</span><span class="sxs-lookup"><span data-stu-id="50058-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="50058-109">قم بالتمرير لأسفل وصولا إلى "البحث عن رسائل البريد الكتروني وحذفها في مؤسستك" للحصول علي مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="50058-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="50058-110">**استدعاء رسالة بريد الكتروني تم إرسالها أو استبدالها**</span><span class="sxs-lookup"><span data-stu-id="50058-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="50058-111">في جزء المجلدات الموجود في الجانب الأيمن من نافذه Outlook ، اختر مجلد العناصر المرسلة.</span><span class="sxs-lookup"><span data-stu-id="50058-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="50058-112">افتح الرسالة التي تريد استدعائها.</span><span class="sxs-lookup"><span data-stu-id="50058-112">Open the message that you want to recall.</span></span> <span data-ttu-id="50058-113">يجب ان تنقر نقرا مزدوجا لفتح الرسالة.</span><span class="sxs-lookup"><span data-stu-id="50058-113">You must double-click to open the message.</span></span> <span data-ttu-id="50058-114">لن يسمح لك تحديد الرسالة بالظهور في جزء القراءة لاستدعاء الرسالة.</span><span class="sxs-lookup"><span data-stu-id="50058-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="50058-115">من علامة التبويب رسالة ، حدد **الإجراءات**  >  **استدعاء هذه الرسالة**.</span><span class="sxs-lookup"><span data-stu-id="50058-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="50058-116">اختر **حذف النسخ غير المقروءة لهذه الرسالة** أو **حذف النسخ غير المقروءة واستبدالها برسالة جديده**، ثم حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="50058-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="50058-117">إذا كنت ترسل رسالة بديله ، فقم بإنشاء الرسالة ، ثم حدد **إرسال**.</span><span class="sxs-lookup"><span data-stu-id="50058-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="50058-118">يتوقف نجاح أو فشل رسالة الاستدعاء علي إعدادات المستلمين في Outlook.</span><span class="sxs-lookup"><span data-stu-id="50058-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="50058-119">لمزيد من المعلومات ، بما في ذلك كيفيه التحقق من الاستدعاء ، راجع [استدعاء رسالة بريد الكتروني التي أرسلتها أو استبدالها](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="50058-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="50058-120">***البحث عن رسائل البريد الكتروني وحذفها في مؤسستك*** للبحث عن رسائل البريد الكتروني وحذفها في مؤسستك ، من الأسهل إذا كنت مسؤولا عاما. إذا لم تكن مسؤولا عاما ، فيجب أضافه حسابك إلى مجموعه ادوار أداره eDiscovery ، أو إلى دور أداره البحث في التوافق.</span><span class="sxs-lookup"><span data-stu-id="50058-120">***Search for and delete email messages in your organization*** To search for and delete email messages in your organization, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="50058-121">لحذف الرسائل ، ستحتاج إلى الانضمام إلى مجموعه ادوار أداره المؤسسة أو البحث وأزاله دور الاداره.</span><span class="sxs-lookup"><span data-stu-id="50058-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="50058-122">يتم تعيين الأذونات لهذه الأدوار في [مركز توافق & الأمان](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="50058-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="50058-123">[إنشاء بحث محتوي](https://docs.microsoft.com/microsoft-365/compliance/content-search) للعثور علي الرسالة التي تريد حذفها.</span><span class="sxs-lookup"><span data-stu-id="50058-123">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="50058-124">[الاتصال بمركز توافق & الأمان PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="50058-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span> 

<span data-ttu-id="50058-125">إذا كنت تستخدم MFA ، فراجع [الاتصال بمركز توافق ال& الأمان ل Microsoft 365 باستخدام مصادقه متعددة العوامل](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="50058-125">If you're using MFA, see [Connect to Microsoft 365 security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span> 
