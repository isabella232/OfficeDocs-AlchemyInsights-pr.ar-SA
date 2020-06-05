---
title: رسائل البريد الإلكتروني المفقودة في الحجر الصحي
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/03/2020
ms.locfileid: "44568890"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="13f15-102">رسائل البريد الإلكتروني المفقودة في الحجر الصحي"</span><span class="sxs-lookup"><span data-stu-id="13f15-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="13f15-103">يمكن للمسؤولين [عرض هذه الرسائل أو إصدارها أو حذفها.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="13f15-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="13f15-104">لفتح مركز التوافق & الأمان، انتقل إلى [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="13f15-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="13f15-105">لفتح صفحة الحجر الصحي مباشرة، انتقل إلى [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="13f15-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="13f15-106">يمكنك البحث حسب القيم التالية:</span><span class="sxs-lookup"><span data-stu-id="13f15-106">You can search by the following values:</span></span>  

- <span data-ttu-id="13f15-107">**معرف الرسالة:** المعرف الفريد للرسالة بشكل عام.</span><span class="sxs-lookup"><span data-stu-id="13f15-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="13f15-108">إذا قمت بتحديد رسالة في القائمة، تظهر قيمة **معرف الرسالة** في جزء **التفاصيل** المنبثقة الذي يظهر.</span><span class="sxs-lookup"><span data-stu-id="13f15-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="13f15-109">يمكن للمسؤولين استخدام [تتبع الرسائل](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) للعثور على الرسائل وقيم معرّف الرسائل المقابلة لها.</span><span class="sxs-lookup"><span data-stu-id="13f15-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="13f15-110">**عنوان البريد الإلكتروني للمرسل:** عنوان البريد الإلكتروني لمرسل واحد.</span><span class="sxs-lookup"><span data-stu-id="13f15-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="13f15-111">**عنوان البريد الإلكتروني للمستلم:** عنوان البريد الإلكتروني لمستلم واحد.</span><span class="sxs-lookup"><span data-stu-id="13f15-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="13f15-112">**الموضوع**: استخدم موضوع الرسالة بأكمله.</span><span class="sxs-lookup"><span data-stu-id="13f15-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="13f15-113">البحث ليس حساساً للحالة.</span><span class="sxs-lookup"><span data-stu-id="13f15-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="13f15-114">بعد إدخال معايير البحث، انقر فوق ![ تحديث زر ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **التحديث** لتصفية النتائج.  </span><span class="sxs-lookup"><span data-stu-id="13f15-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="13f15-115">cmdlets التي تستخدمها لعرض وإدارة الرسائل والملفات في الحجر الصحي هي:</span><span class="sxs-lookup"><span data-stu-id="13f15-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="13f15-116">حذف-العزلرسالة</span><span class="sxs-lookup"><span data-stu-id="13f15-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="13f15-117">رسالة التصدير والحجر الصحي</span><span class="sxs-lookup"><span data-stu-id="13f15-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="13f15-118">الحصول على الحجر الصحيرسالة</span><span class="sxs-lookup"><span data-stu-id="13f15-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="13f15-119">[معاينة الحجرالصحيرسالة](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): لاحظ أن هذا cmdlet هو فقط للرسائل ، وليس ملفات البرامج الضارة من ATP لSharePoint أون لاين ، OneDrive للأعمال التجارية ، أو فرق.</span><span class="sxs-lookup"><span data-stu-id="13f15-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="13f15-120">رسالة الإصدار-الحجر الصحي</span><span class="sxs-lookup"><span data-stu-id="13f15-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)