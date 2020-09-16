---
title: مجلد 1336 ريكوفيرابليتيمس ممتلئ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741254"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="a4f5f-102">المجلد "العناصر القابلة للاسترداد" ممتلئ</span><span class="sxs-lookup"><span data-stu-id="a4f5f-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="a4f5f-103">بالنسبة إلى علب بريد Exchange Online ، يكون حد التخزين الافتراضي لمجلد العناصر القابلة للاسترداد هو 30 غيغابايت.</span><span class="sxs-lookup"><span data-stu-id="a4f5f-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="a4f5f-104">تتم زيادة حد مساحة التخزين لمجلد العناصر القابلة للاسترداد تلقائيا إلى 100 غيغابايت إذا تم وضع علبه البريد في احتجاز دعوى قضائية ، أو احتجاز eDiscovery ، أو تم تعيينه لنهج استبقاء.</span><span class="sxs-lookup"><span data-stu-id="a4f5f-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="a4f5f-105">عند وصول مجلد "العناصر القابلة للاسترداد" إلى حد التخزين ، تتاثر وظيفة علبه البريد بالطرق التالية:</span><span class="sxs-lookup"><span data-stu-id="a4f5f-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="a4f5f-106">لا يمكن للمستخدم حذف العناصر من علبه البريد.</span><span class="sxs-lookup"><span data-stu-id="a4f5f-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="a4f5f-107">لا يمكن لمساعد المجلد المدار حذف العناصر بالاستناد إلى علامة الاستبقاء أو إعدادات المجلد المدار.</span><span class="sxs-lookup"><span data-stu-id="a4f5f-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="a4f5f-108">بالنسبة لعلب البريد التي تم تمكين استرداد العناصر الفردية فيها أو وضعها قيد الاحتجاز ، لا يمكن لعمليه الحماية في الصفحة الخاصة بالنسخ والكتابة الاحتفاظ بإصدارات العناصر التي قام المستخدم بتحريرها.</span><span class="sxs-lookup"><span data-stu-id="a4f5f-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="a4f5f-109">بالنسبة لعلب البريد التي تم تمكين تسجيل تدقيق علبه البريد لها ، يمكن حفظ إدخالات سجل تدقيق علبه البريد في المجلد الفرعي لعمليات التدقيق في المجلد "العناصر القابلة للاسترداد".</span><span class="sxs-lookup"><span data-stu-id="a4f5f-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="a4f5f-110">بالنسبة لعلب البريد غير الموجودة في وضع الانتظار ، يمكن `Search-Mailbox -SearchDumpsterOnly -DeleteContent` للمسؤولين استخدام الأمر في Exchange Online PowerShell لحذف العناصر الموجودة في مجلد العناصر القابلة للاسترداد.</span><span class="sxs-lookup"><span data-stu-id="a4f5f-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="a4f5f-111">لمزيد من المعلومات، راجع المواضيع التالية:</span><span class="sxs-lookup"><span data-stu-id="a4f5f-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="a4f5f-112">البحث عن الرسائل وحذفها</span><span class="sxs-lookup"><span data-stu-id="a4f5f-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="a4f5f-113">البحث-علبه البريد</span><span class="sxs-lookup"><span data-stu-id="a4f5f-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="a4f5f-114">بالنسبة لعلب البريد قيد الانتظار ، يجب علي المسؤولين أزاله التعليق قبل ان يتمكنوا من حذف العناصر من مجلد "العناصر القابلة للاسترداد".</span><span class="sxs-lookup"><span data-stu-id="a4f5f-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="a4f5f-115">لمزيد من المعلومات ، راجع [حذف العناصر في مجلد "العناصر القابلة للاسترداد" من علب البريد المستندة إلى السحابة قيد الانتظار](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="a4f5f-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="a4f5f-116">للمساعدة علي منع المجلد "العناصر القابلة للاسترداد" من الامتلاء ، يمكن للمسؤولين زيادة حد مساحة التخزين لمجلد "العناصر القابلة للاسترداد" لعلب البريد واعداد نهج استبقاء علبه البريد الذي ينقل العناصر من مجلد "العناصر القابلة للاسترداد" إلى علبه بريد الأرشيف الخاصة بالمستخدم.</span><span class="sxs-lookup"><span data-stu-id="a4f5f-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="a4f5f-117">راجع [زيادة الحصة النسبية للعناصر القابلة للاسترداد لعلب البريد قيد الانتظار](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="a4f5f-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
