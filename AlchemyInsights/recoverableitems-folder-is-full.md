---
title: 1336 ريكوفيرابليتيمس المجلد ممتلئ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 8a5859ba29d847606e8b44d169c3cd6a26364744
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36509710"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="96b31-102">امتلاء المجلد "العناصر القابلة للاسترداد"</span><span class="sxs-lookup"><span data-stu-id="96b31-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="96b31-103">علب بريد Exchange عبر الإنترنت في Office 365، حد التخزين الافتراضي للمجلد "العناصر القابلة للاسترداد" بالنسبة سعة 30 جيجابايت.</span><span class="sxs-lookup"><span data-stu-id="96b31-103">For Exchange Online mailboxes in Office 365, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="96b31-104">حد التخزين للمجلد "العناصر القابلة للاسترداد" تلقائياً تزداد إلى 100 جيجابايت حالة علبة البريد على "إجراء التقاضي"، اضغط eDiscovery، أو يتم تعيين نهج استبقاء Office 365.</span><span class="sxs-lookup"><span data-stu-id="96b31-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to an Office 365 retention policy.</span></span>

<span data-ttu-id="96b31-105">عندما يصل المجلد "العناصر القابلة للاسترداد" إلى حد التخزين، تتأثر وظيفة علبة البريد بالطرق التالية:</span><span class="sxs-lookup"><span data-stu-id="96b31-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="96b31-106">يتعذر على المستخدم حذف العناصر من علبة البريد.</span><span class="sxs-lookup"><span data-stu-id="96b31-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="96b31-107">لا يمكن حذف "مجلد مساعد المدار" العناصر استناداً إلى إعدادات المجلدات المدارة أو علامة استبقاء.</span><span class="sxs-lookup"><span data-stu-id="96b31-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="96b31-108">علب البريد التي تمكين استرداد عنصر واحد أو وضعه قيد الإيقاف، لا الاحتفاظ بإصدارات العناصر التي يقوم المستخدم بتحرير عملية حماية الصفحة النسخ عند الكتابة.</span><span class="sxs-lookup"><span data-stu-id="96b31-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="96b31-109">علب البريد التي تحتوي على علبة البريد تسجيل تمكين التدقيق، يمكن حفظ لم إدخالات سجل التدقيق علبة البريد في مجلد فرعي عمليات مراجعة الحسابات في مجلد "العناصر القابلة للاسترداد".</span><span class="sxs-lookup"><span data-stu-id="96b31-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="96b31-110">يمكن استخدام المسؤولين لصناديق البريد التي ليست قيد الاحتجاز، `Search-Mailbox -SearchDumpsterOnly -DeleteContent` في PowerShell Exchange عبر إنترنت حذف العناصر الموجودة في المجلد "العناصر القابلة للاسترداد".</span><span class="sxs-lookup"><span data-stu-id="96b31-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="96b31-111">لمزيد من المعلومات، راجع المواضيع التالية:</span><span class="sxs-lookup"><span data-stu-id="96b31-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="96b31-112">البحث عن الرسائل وحذفها</span><span class="sxs-lookup"><span data-stu-id="96b31-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="96b31-113">صندوق بريد البحث</span><span class="sxs-lookup"><span data-stu-id="96b31-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="96b31-114">علب البريد قيد الانتظار، يلزم المسؤولين إزالة الاحتجاز قبل أن يتمكنوا من العناصر المحذوفة من مجلد "العناصر القابلة للاسترداد".</span><span class="sxs-lookup"><span data-stu-id="96b31-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="96b31-115">لمزيد من المعلومات، راجع [حذف العناصر الموجودة في المجلد من صناديق البريد المستندة إلى مجموعة النظراء على عقد "العناصر القابلة للاسترداد"](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="96b31-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="96b31-116">زيادة حد التخزين من "العناصر القابلة للاسترداد" المجلد لعلب بريد على عقد وإعداد نهج استبقاء علبة بريد نقل العناصر من مجلد "العناصر القابلة للاسترداد" للأرشيف المستخدم للمساعدة في الحيلولة دون تحول كامل في مجلد "العناصر القابلة للاسترداد"، المسؤولين علبة البريد.</span><span class="sxs-lookup"><span data-stu-id="96b31-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="96b31-117">راجع [زيادة الحصة النسبية لعلب بريد على عقد "العناصر القابلة للاسترداد"](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="96b31-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
