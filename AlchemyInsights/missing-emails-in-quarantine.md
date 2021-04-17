---
title: رسائل البريد الإلكتروني المفقودة في الفحص
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
- "5668"
- "9002625"
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831721"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="87c1a-102">رسائل البريد الإلكتروني المفقودة في الفحص"</span><span class="sxs-lookup"><span data-stu-id="87c1a-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="87c1a-103">يمكن للمسؤولين [عرض هذه الرسائل أو إصدارها أو حذفها.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="87c1a-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="87c1a-104">لفتح مركز التوافق &، انتقل إلى [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="87c1a-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="87c1a-105">لفتح صفحة الفحص مباشرة، انتقل إلى [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="87c1a-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="87c1a-106">يمكنك البحث حسب القيم التالية:</span><span class="sxs-lookup"><span data-stu-id="87c1a-106">You can search by the following values:</span></span>  

- <span data-ttu-id="87c1a-107">**معرف الرسالة**: المعرف الفريد العام للرسالة.</span><span class="sxs-lookup"><span data-stu-id="87c1a-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="87c1a-108">إذا حددت رسالة في القائمة، تظهر القيمة **"معرّف** الرسالة" في جزء القائمة من خلال التفاصيل التي تظهر. </span><span class="sxs-lookup"><span data-stu-id="87c1a-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="87c1a-109">يمكن للمسؤولين [استخدام تتبع الرسائل](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) للعثور على الرسائل وقيمها المطابقة لمعرف الرسالة.</span><span class="sxs-lookup"><span data-stu-id="87c1a-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="87c1a-110">**عنوان البريد الإلكتروني المرسل:** عنوان البريد الإلكتروني لمرسل واحد.</span><span class="sxs-lookup"><span data-stu-id="87c1a-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="87c1a-111">**عنوان البريد الإلكتروني للمستلم**: عنوان البريد الإلكتروني لمستلم واحد.</span><span class="sxs-lookup"><span data-stu-id="87c1a-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="87c1a-112">**الموضوع**: استخدم الموضوع بالكامل للرسالة.</span><span class="sxs-lookup"><span data-stu-id="87c1a-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="87c1a-113">لا يتحسس البحث حالة التحسس.</span><span class="sxs-lookup"><span data-stu-id="87c1a-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="87c1a-114">بعد إدخال معايير البحث، انقر فوق الزر ![ تحديث ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **تحديث** لتصفية النتائج.  </span><span class="sxs-lookup"><span data-stu-id="87c1a-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="87c1a-115">إن cmdlets التي تستخدمها لعرض الرسائل والملفات وإدارتها في الفحص هي:</span><span class="sxs-lookup"><span data-stu-id="87c1a-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="87c1a-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="87c1a-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="87c1a-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="87c1a-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="87c1a-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="87c1a-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="87c1a-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): لاحظ أن أمر cmdlet هذا للرسائل فقط، وليس ملفات البرامج الضارة من ATP ل SharePoint Online أو OneDrive for Business أو Teams.</span><span class="sxs-lookup"><span data-stu-id="87c1a-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="87c1a-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="87c1a-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)