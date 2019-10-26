---
title: استدعاء سطح مكتب Outlook أو استبدال رسالة بريد الكتروني
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/25/2019
ms.locfileid: "36496098"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="9894b-102">استدعاء أو استبدال رسالة بريد الكتروني Outlook</span><span class="sxs-lookup"><span data-stu-id="9894b-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="9894b-103">كما المشرف ، يمكنك **استدعاء الرسائل نيابة عن المستخدمين باستخدام PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="9894b-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="9894b-104">لا يمكنك تذكر الرسائل من مركز الاداره.</span><span class="sxs-lookup"><span data-stu-id="9894b-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="9894b-105">يمكنك **فقط استدعاء الرسائل التي يتم إرسالها إلى الأشخاص في المؤسسة الخاصة بك**.</span><span class="sxs-lookup"><span data-stu-id="9894b-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="9894b-106">إذا تم إرسال الرسالة إلى عنوان Gmail ، علي سبيل المثال ، لا يمكنك تذكر ذلك.</span><span class="sxs-lookup"><span data-stu-id="9894b-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="9894b-107">يمكنك **فقط استدعاء الرسائل المرسلة من Outlook 2016 علي جهاز الكمبيوتر**.</span><span class="sxs-lookup"><span data-stu-id="9894b-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="9894b-108">إذا قام مستخدم بإرسال رسالة باستخدام Outlook لنظام التشغيل Mac أو Outlook علي الويب ، لا يمكنك تذكر ذلك.</span><span class="sxs-lookup"><span data-stu-id="9894b-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="9894b-109">لاستدعاء رسالة بريد الكتروني أو استبدالها:</span><span class="sxs-lookup"><span data-stu-id="9894b-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="9894b-110">في جزء المجلد علي يسار اطار Outlook ، حدد مجلد "العناصر المرسلة".</span><span class="sxs-lookup"><span data-stu-id="9894b-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="9894b-111">انقر نقرا مزدوجا فوق الرسالة التي تريد استدعاءها لفتحها.</span><span class="sxs-lookup"><span data-stu-id="9894b-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="9894b-112">حدد علامة التبويب **رسالة** ثم حدد **الإجراءات** > **استدعاء هذه الرسالة**.</span><span class="sxs-lookup"><span data-stu-id="9894b-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="9894b-113">حدد **حذف النسخ غير المقروءة من هذه الرسالة** أو **احذف النسخ غير المقروءة واستبدلها برسالة جديده**، ثم حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="9894b-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="9894b-114">إذا كنت ترسل رسالة بديله ، فقم بإنشاء الرسالة ، ثم حدد **إرسال**.</span><span class="sxs-lookup"><span data-stu-id="9894b-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="9894b-115">نجاح أو فشل استدعاء رسالة يعتمد علي إعدادات المستلم في Outlook.</span><span class="sxs-lookup"><span data-stu-id="9894b-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="9894b-116">للحصول علي خطوات للتحقق من استدعاء ، راجع [هذه المقالة](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="9894b-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="9894b-117">البحث عن رسائل البريد الكتروني وحذفها في مؤسستك</span><span class="sxs-lookup"><span data-stu-id="9894b-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="9894b-118">إذا لم تكن مسؤولا عموميا ، فيجب أضافه حسابك إلى دور مدير eDiscovery أو دور أداره بحث التوافق للبحث عن الرسائل.</span><span class="sxs-lookup"><span data-stu-id="9894b-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="9894b-119">لحذف الرسائل ، ستحتاج إلى الانضمام إلى مجموعه دور أداره المؤسسة أو دور أداره البحث والازاله.</span><span class="sxs-lookup"><span data-stu-id="9894b-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="9894b-120">يتم تعيين الأذونات لهذه الأدوار في [مركز الأمان والتوافق](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="9894b-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="9894b-121">[إنشاء بحث محتوي](https://docs.microsoft.com/office365/securitycompliance/content-search) للعثور علي الرسالة التي تريد حذفها.</span><span class="sxs-lookup"><span data-stu-id="9894b-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="9894b-122">[الاتصال بمركز الأمان والتوافق PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="9894b-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="9894b-123">إذا كنت تستخدم المصادقة متعددة العوامل ، راجع [الاتصال ب Office 365 الأمان ومركز التوافق PowerShell باستخدام مصادقه متعددة العوامل](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="9894b-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>