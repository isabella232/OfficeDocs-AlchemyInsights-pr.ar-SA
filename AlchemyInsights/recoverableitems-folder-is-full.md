---
title: 1336 مجلد العناصر القابلة للاسترداد ممتلئ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: fb10b792981040bdcf4661b8aff30733c2438212
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720239"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="bfebe-102">مجلد العناصر القابلة للاسترداد ممتلئ</span><span class="sxs-lookup"><span data-stu-id="bfebe-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="bfebe-103">بالنسبة لصناديق بريد Exchange Online، يكون حد التخزين الافتراضي لمجلد العناصر القابلة للاسترداد هو 30 غيغابايت.</span><span class="sxs-lookup"><span data-stu-id="bfebe-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="bfebe-104">يتم زيادة حد التخزين لمجلد العناصر القابلة للاسترداد تلقائيًا إلى 100 غيغابايت إذا تم وضع علبة البريد في "عقد التقاضي" أو "احتجاز eDiscovery" أو تم تعيينه إلى نهج الاحتفاظ.</span><span class="sxs-lookup"><span data-stu-id="bfebe-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="bfebe-105">عندما يصل مجلد العناصر القابلة للاسترداد إلى حد التخزين، تتأثر وظيفة علبة البريد بالطرق التالية:</span><span class="sxs-lookup"><span data-stu-id="bfebe-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="bfebe-106">لا يمكن للمستخدم حذف العناصر من علبة البريد.</span><span class="sxs-lookup"><span data-stu-id="bfebe-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="bfebe-107">لا يمكن لمساعد المجلد المدار حذف العناصر استنادًا إلى علامة الاحتفاظ أو إعدادات المجلد المدارة.</span><span class="sxs-lookup"><span data-stu-id="bfebe-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="bfebe-108">بالنسبة لصناديق البريد التي تم تمكين استرداد العنصر الواحد أو يتم وضعها في الانتظار، لا يمكن لعملية حماية صفحة النسخ على الكتابة الاحتفاظ بإصدارات العناصر التي تم تحريرها من قبل المستخدم.</span><span class="sxs-lookup"><span data-stu-id="bfebe-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="bfebe-109">بالنسبة لصناديق البريد التي تم تمكين تسجيل تدقيق علبة البريد، لا يمكن حفظ إدخالات سجل تدقيق علبة البريد في المجلد الفرعي للتدقيقات في مجلد العناصر القابلة للاسترداد.</span><span class="sxs-lookup"><span data-stu-id="bfebe-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="bfebe-110">بالنسبة لصناديق البريد غير المعلّقة، `Search-Mailbox -SearchDumpsterOnly -DeleteContent` يمكن للمسؤولين استخدام الأمر في Exchange Online PowerShell لحذف العناصر الموجودة في مجلد العناصر القابلة للاسترداد.</span><span class="sxs-lookup"><span data-stu-id="bfebe-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="bfebe-111">لمزيد من المعلومات، راجع المواضيع التالية:</span><span class="sxs-lookup"><span data-stu-id="bfebe-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="bfebe-112">البحث عن الرسائل وحذفها</span><span class="sxs-lookup"><span data-stu-id="bfebe-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="bfebe-113">البحث - علبة البريد</span><span class="sxs-lookup"><span data-stu-id="bfebe-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="bfebe-114">بالنسبة لصناديق البريد التي هي في الانتظار، يجب على المسؤولين إزالة الانتظار قبل أن يتمكنوا من حذف العناصر من مجلد العناصر القابلة للاسترداد.</span><span class="sxs-lookup"><span data-stu-id="bfebe-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="bfebe-115">لمزيد من المعلومات، راجع [حذف العناصر الموجودة في مجلد العناصر القابلة للاسترداد لصناديق البريد المستندة إلى مجموعة النظراء الموجودة في الانتظار](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="bfebe-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="bfebe-116">للمساعدة في منع مجلد العناصر القابلة للاسترداد من أن يصبح ممتلئًا، يمكن للمسؤولين زيادة حد التخزين لمجلد العناصر القابلة للاسترداد لصناديق البريد قيد الانتظار وإعداد نهج الاحتفاظ بعلبة البريد الذي ينقل العناصر من مجلد العناصر القابلة للاسترداد إلى صندوق بريد أرشيف المستخدم.</span><span class="sxs-lookup"><span data-stu-id="bfebe-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="bfebe-117">راجع [زيادة حصة العناصر القابلة للاسترداد لصناديق البريد في الانتظار](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="bfebe-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
