---
title: استكشاف الأخطاء وإصلاحها الأحداث من البريد الإلكتروني
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44568877"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="36c1d-102">استكشاف الأخطاء وإصلاحها الأحداث من البريد الإلكتروني</span><span class="sxs-lookup"><span data-stu-id="36c1d-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="36c1d-103">التحقق من تمكين الميزة لصندوق البريد: \*\*Get-EventsFromEmailConfiguration-الهوية <mailbox> \*\*</span><span class="sxs-lookup"><span data-stu-id="36c1d-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="36c1d-104">ثم ننظر في 'الأحداث من البريد الإلكتروني' سجلات **تصدير-MailboxDiagnosticLogs <mailbox> -مكون TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="36c1d-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="36c1d-105">في سجلات "الأحداث من البريد الإلكتروني"، ابحث عن InternetMessageId الذي يطابق العنصر في علبة البريد.</span><span class="sxs-lookup"><span data-stu-id="36c1d-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="36c1d-106">يحدد TrustScore ما إذا تمت إضافة العنصر أم لا.</span><span class="sxs-lookup"><span data-stu-id="36c1d-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="36c1d-107">سيتم إضافة الأحداث فقط إذا كان TrustScore = "موثوق به".</span><span class="sxs-lookup"><span data-stu-id="36c1d-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="36c1d-108">يتم تحديد نقاط الثقة بواسطة خصائص SPF أو Dkim أو Dmarc الموجودة في رأس الرسالة.</span><span class="sxs-lookup"><span data-stu-id="36c1d-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="36c1d-109">لعرض هذه الخصائص:</span><span class="sxs-lookup"><span data-stu-id="36c1d-109">To view these properties:</span></span>

<span data-ttu-id="36c1d-110">**توقعات سطح المكتب**</span><span class="sxs-lookup"><span data-stu-id="36c1d-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="36c1d-111">فتح العنصر</span><span class="sxs-lookup"><span data-stu-id="36c1d-111">Open the item</span></span>
- <span data-ttu-id="36c1d-112">خصائص > الملف -> رؤوس إنترنت</span><span class="sxs-lookup"><span data-stu-id="36c1d-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="36c1d-113">او</span><span class="sxs-lookup"><span data-stu-id="36c1d-113">or</span></span>

<span data-ttu-id="36c1d-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="36c1d-114">**MFCMapi**</span></span>

- <span data-ttu-id="36c1d-115">الانتقال إلى العنصر الموجود في البريد الوارد</span><span class="sxs-lookup"><span data-stu-id="36c1d-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="36c1d-116">ابحث عن PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="36c1d-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="36c1d-117">يتم تحديد هذه الخصائص وتسجيلها أثناء النقل والتوجيه.</span><span class="sxs-lookup"><span data-stu-id="36c1d-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="36c1d-118">لمزيد من استكشاف الأخطاء وإصلاحها، قد تحتاج إلى متابعة مع دعم النقل حول الفشل في SPF و DKIM و.أو DMARC.</span><span class="sxs-lookup"><span data-stu-id="36c1d-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>