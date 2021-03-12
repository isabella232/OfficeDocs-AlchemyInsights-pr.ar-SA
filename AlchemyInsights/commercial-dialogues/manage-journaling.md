---
title: إدارة دفاتر اليومية
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004299"
- "7677"
ms.openlocfilehash: 2fcd0f386d2da8cad19fcc9872482bb75fe00dd2
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743052"
---
# <a name="manage-journaling"></a><span data-ttu-id="e2f61-102">إدارة دفاتر اليومية</span><span class="sxs-lookup"><span data-stu-id="e2f61-102">Manage journaling</span></span>

<span data-ttu-id="e2f61-103">يمكن أن تساعد دفاتر اليومية مؤسستك على الاستجابة لمتطلبات التوافق القانوني والتنظيمي والتنظيمي من خلال تسجيل اتصالات البريد الإلكتروني الواردة والداخلة.</span><span class="sxs-lookup"><span data-stu-id="e2f61-103">Journaling can help your organization respond to legal, regulatory, and organizational compliance requirements by recording inbound and outbound email communications.</span></span> <span data-ttu-id="e2f61-104">ضع في اعتبارك:</span><span class="sxs-lookup"><span data-stu-id="e2f61-104">Keep in mind:</span></span>

* <span data-ttu-id="e2f61-105">يجب أن يكون لديك [أذونات إدارة المؤسسة](https://go.microsoft.com/fwlink/?linkid=2115259) وإدارة [السجلات](https://go.microsoft.com/fwlink/?linkid=2115469) قبل أن تتمكن من إدارة دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="e2f61-105">You need to have [Organization Management](https://go.microsoft.com/fwlink/?linkid=2115259) and [Records Management](https://go.microsoft.com/fwlink/?linkid=2115469) permissions before you can manage journaling.</span></span>
* <span data-ttu-id="e2f61-106">يجب أن يكون لديك علبة بريد دفتر يومية و(بشكل اختياري) علبة بريد دفتر يومية بديلة مكونة.</span><span class="sxs-lookup"><span data-stu-id="e2f61-106">You need to have a journal mailbox and (optionally) an alternate journaling mailbox configured.</span></span> <span data-ttu-id="e2f61-107">لمعرفة المزيد، راجع [تكوين دفتر اليومية في Exchange Online](https://go.microsoft.com/fwlink/?linkid=2115260).</span><span class="sxs-lookup"><span data-stu-id="e2f61-107">To learn more, see [Configure Journaling in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2115260).</span></span>
* <span data-ttu-id="e2f61-108">في Exchange Online، يوجد حد لعدد قواعد دفتر اليومية التي يمكنك إنشاؤها.</span><span class="sxs-lookup"><span data-stu-id="e2f61-108">In Exchange Online, there's a limit to the number of journal rules that you can create.</span></span> <span data-ttu-id="e2f61-109">للحصول على التفاصيل، راجع حدود قواعد دفتر [اليومية والنقل علبة الوارد](https://go.microsoft.com/fwlink/?linkid=2115261).</span><span class="sxs-lookup"><span data-stu-id="e2f61-109">For details, see [Journal, transport, and inbox rule limits](https://go.microsoft.com/fwlink/?linkid=2115261).</span></span>
* <span data-ttu-id="e2f61-110">لا يدعم Exchange Online تسليم تقارير دفتر اليومية إلى علبة بريد Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="e2f61-110">Exchange Online doesn't support delivering journal reports to an Exchange Online mailbox.</span></span> <span data-ttu-id="e2f61-111">يجب تحديد عنوان البريد الإلكتروني لنظام أرشفة موقع أو خدمة أرشفة جهة خارجية كعميل بريد دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="e2f61-111">You must specify the email address of an on-premises archiving system or a third-party archiving service as the journaling mailbox.</span></span>
