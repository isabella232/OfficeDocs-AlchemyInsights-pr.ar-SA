---
title: رسائل البريد الكتروني المفقودة في الفحص
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
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673701"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="ade00-102">رسائل البريد الكتروني المفقودة في الفحص "</span><span class="sxs-lookup"><span data-stu-id="ade00-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="ade00-103">يمكن للمسؤولين [عرض هذه الرسائل أو تحريرها أو حذفها.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="ade00-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="ade00-104">لفتح مركز توافق & الأمان ، انتقل إلى [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="ade00-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="ade00-105">لفتح صفحه الفحص مباشره ، انتقل إلى [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="ade00-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="ade00-106">يمكنك البحث بحسب القيم التالية:</span><span class="sxs-lookup"><span data-stu-id="ade00-106">You can search by the following values:</span></span>  

- <span data-ttu-id="ade00-107">**معرف الرسالة**: المعرف الفريد العمومي للرسالة.</span><span class="sxs-lookup"><span data-stu-id="ade00-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="ade00-108">إذا قمت بتحديد رسالة في القائمة ، ستظهر قيمه  **معرف الرسالة**  في جزء  **التفاصيل**  المنبثق الذي يظهر.</span><span class="sxs-lookup"><span data-stu-id="ade00-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="ade00-109">يمكن للمسؤولين استخدام [تتبع الرسائل](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) للبحث عن الرسائل وقيم معرف الرسائل المقابلة لها.</span><span class="sxs-lookup"><span data-stu-id="ade00-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="ade00-110">**عنوان البريد الكتروني**للمرسل: عنوان البريد الكتروني الخاص بالمرسل.</span><span class="sxs-lookup"><span data-stu-id="ade00-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="ade00-111">**عنوان البريد الكتروني للمستلم**: عنوان البريد الكتروني الخاص بمستلم واحد.</span><span class="sxs-lookup"><span data-stu-id="ade00-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="ade00-112">**الموضوع**: استخدم الموضوع بالبالكامل في الرسالة.</span><span class="sxs-lookup"><span data-stu-id="ade00-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="ade00-113">لا يكون البحث متحسسا لحاله الأحرف.</span><span class="sxs-lookup"><span data-stu-id="ade00-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="ade00-114">بعد إدخال معايير البحث ، انقر فوق ![ الزر تحديث ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** التحديث لتصفيه النتائج.  </span><span class="sxs-lookup"><span data-stu-id="ade00-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="ade00-115">أوامر cmdlets التي تستخدمها لعرض الرسائل والملفات وأدارتها في الفحص هي:</span><span class="sxs-lookup"><span data-stu-id="ade00-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="ade00-116">Delete-قوارانتينيميساجي</span><span class="sxs-lookup"><span data-stu-id="ade00-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="ade00-117">تصدير-قوارانتينيميساجي</span><span class="sxs-lookup"><span data-stu-id="ade00-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="ade00-118">قوارانتينيميساجي</span><span class="sxs-lookup"><span data-stu-id="ade00-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="ade00-119">[معاينه-قوارانتينيميساجي](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): لاحظ ان أمر cmdlet هذا للرسائل فقط ، وليس الملفات الضارة من ATP ل SharePoint Online أو OneDrive for business أو الفرق.</span><span class="sxs-lookup"><span data-stu-id="ade00-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="ade00-120">الإصدار-قوارانتينيميساجي</span><span class="sxs-lookup"><span data-stu-id="ade00-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)