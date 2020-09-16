---
title: استكشاف الأخطاء وإصلاحها من البريد الكتروني
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658721"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="8a080-102">استكشاف الأخطاء وإصلاحها من البريد الكتروني</span><span class="sxs-lookup"><span data-stu-id="8a080-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="8a080-103">تاكد من تمكين الميزة لعلبه البريد: **الحصول علي افينتسفروميميلكونفيجوريشن <mailbox> الهوية**</span><span class="sxs-lookup"><span data-stu-id="8a080-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="8a080-104">ثم انظر علي سجلات "الاحداث من **البريد الكتروني" التصدير-ميلبوكسدياجنوستيكلوجس <mailbox> -مكون تيميبروفيلي**</span><span class="sxs-lookup"><span data-stu-id="8a080-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="8a080-105">في سجلات "الاحداث من البريد الكتروني" ، ابحث عن إينتيرنيتميساجيد الذي يتطابق مع العنصر في علبه البريد.</span><span class="sxs-lookup"><span data-stu-id="8a080-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="8a080-106">يحدد تروستسكوري ما إذا تمت أضافه العنصر ام لا.</span><span class="sxs-lookup"><span data-stu-id="8a080-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="8a080-107">ستتم أضافه الاحداث فقط إذا كانت تروستسكوري = "موثوق بها".</span><span class="sxs-lookup"><span data-stu-id="8a080-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="8a080-108">يتم تحديد تروستسكوري بواسطة SPF أو Dkim أو Dmarc الخصائص ، وهي موجودة في راس الرسالة.</span><span class="sxs-lookup"><span data-stu-id="8a080-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="8a080-109">لعرض الخصائص التالية:</span><span class="sxs-lookup"><span data-stu-id="8a080-109">To view these properties:</span></span>

<span data-ttu-id="8a080-110">**سطح المكتب Outlook**</span><span class="sxs-lookup"><span data-stu-id="8a080-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="8a080-111">فتح العنصر</span><span class="sxs-lookup"><span data-stu-id="8a080-111">Open the item</span></span>
- <span data-ttu-id="8a080-112">خصائص الملفات >-> رؤوس الإنترنت</span><span class="sxs-lookup"><span data-stu-id="8a080-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="8a080-113">or</span><span class="sxs-lookup"><span data-stu-id="8a080-113">or</span></span>

<span data-ttu-id="8a080-114">**مفكمابي**</span><span class="sxs-lookup"><span data-stu-id="8a080-114">**MFCMapi**</span></span>

- <span data-ttu-id="8a080-115">الانتقال إلى العنصر الموجود في علبه الوارد</span><span class="sxs-lookup"><span data-stu-id="8a080-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="8a080-116">البحث عن PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="8a080-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="8a080-117">يتم تحديد هذه الخصائص وتسجيلها اثناء النقل والتوجيه.</span><span class="sxs-lookup"><span data-stu-id="8a080-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="8a080-118">لمزيد من استكشاف الأخطاء وإصلاحها ، قد تحتاج إلى متابعه دعم النقل حول حالات الفشل في SPF و DKIM و. أو DMARC.</span><span class="sxs-lookup"><span data-stu-id="8a080-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>