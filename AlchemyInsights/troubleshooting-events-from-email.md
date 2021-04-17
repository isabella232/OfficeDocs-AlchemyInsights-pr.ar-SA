---
title: استكشاف الأخطاء في الأحداث وإصلاحها من البريد الإلكتروني
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834826"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="8e098-102">استكشاف الأخطاء في الأحداث وإصلاحها من البريد الإلكتروني</span><span class="sxs-lookup"><span data-stu-id="8e098-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="8e098-103">التحقق من تمكين الميزة لعلبة البريد: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span><span class="sxs-lookup"><span data-stu-id="8e098-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="8e098-104">ثم انظر إلى سجلات 'الأحداث من البريد الإلكتروني' **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="8e098-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="8e098-105">في سجلات "الأحداث من البريد الإلكتروني"، ابحث عن InternetMessageId الذي يتطابق مع العنصر في علبة البريد.</span><span class="sxs-lookup"><span data-stu-id="8e098-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="8e098-106">يحدد TrustScore ما إذا كان العنصر مضافا أم لا.</span><span class="sxs-lookup"><span data-stu-id="8e098-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="8e098-107">لن تضاف الأحداث إلا إذا كانت TrustScore = "موثوق به".</span><span class="sxs-lookup"><span data-stu-id="8e098-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="8e098-108">يتم تحديد TrustScore بواسطة خصائص SPF أو Dkim أو Dmarc، والتي توجد في رأس الرسالة.</span><span class="sxs-lookup"><span data-stu-id="8e098-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="8e098-109">لعرض هذه الخصائص:</span><span class="sxs-lookup"><span data-stu-id="8e098-109">To view these properties:</span></span>

<span data-ttu-id="8e098-110">**Outlook لسطح المكتب**</span><span class="sxs-lookup"><span data-stu-id="8e098-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="8e098-111">فتح العنصر</span><span class="sxs-lookup"><span data-stu-id="8e098-111">Open the item</span></span>
- <span data-ttu-id="8e098-112">File -> Properties -> رؤوس الإنترنت</span><span class="sxs-lookup"><span data-stu-id="8e098-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="8e098-113">أو</span><span class="sxs-lookup"><span data-stu-id="8e098-113">or</span></span>

<span data-ttu-id="8e098-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="8e098-114">**MFCMapi**</span></span>

- <span data-ttu-id="8e098-115">الانتقال إلى العنصر في علبة الوارد</span><span class="sxs-lookup"><span data-stu-id="8e098-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="8e098-116">ابحث عن PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="8e098-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="8e098-117">يتم تحديد هذه الخصائص ويتم تسجيلها أثناء النقل التوجيه.</span><span class="sxs-lookup"><span data-stu-id="8e098-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="8e098-118">لمزيد من استكشاف الأخطاء وإصلاحها، قد تحتاج إلى المتابعة مع دعم النقل حول حالات الفشل في SPF أو DKIM و.أو DMARC.</span><span class="sxs-lookup"><span data-stu-id="8e098-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>