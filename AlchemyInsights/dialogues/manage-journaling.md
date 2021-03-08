---
title: إدارة دفتر اليومية
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
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523190"
---
# <a name="manage-journaling"></a><span data-ttu-id="28d9a-102">إدارة دفاتر اليومية</span><span class="sxs-lookup"><span data-stu-id="28d9a-102">Manage journaling</span></span>

<span data-ttu-id="28d9a-103">يمكن أن يساعد العمل اليومية مؤسستك على الاستجابة لمتطلبات التوافق التنظيمية والقانونية والتنظيمية من خلال تسجيل مراسلات البريد الإلكتروني الواردة وال الصادرة.</span><span class="sxs-lookup"><span data-stu-id="28d9a-103">Journaling can help your organization respond to legal, regulatory, and organizational compliance requirements by recording inbound and outbound email communications.</span></span> <span data-ttu-id="28d9a-104">ضع في اعتبارك:</span><span class="sxs-lookup"><span data-stu-id="28d9a-104">Keep in mind:</span></span>

* <span data-ttu-id="28d9a-105">يجب أن يكون لديك [أذونات إدارة المؤسسة](https://go.microsoft.com/fwlink/?linkid=2115259) وإدارة [السجلات](https://go.microsoft.com/fwlink/?linkid=2115469) قبل أن تتمكن من إدارة دفتر اليومية.</span><span class="sxs-lookup"><span data-stu-id="28d9a-105">You need to have [Organization Management](https://go.microsoft.com/fwlink/?linkid=2115259) and [Records Management](https://go.microsoft.com/fwlink/?linkid=2115469) permissions before you can manage journaling.</span></span>
* <span data-ttu-id="28d9a-106">يجب أن يكون لديك علبة بريد دفتر يومية و(اختياريا) علبة بريد بديلة لدفاتر اليومية مكونة.</span><span class="sxs-lookup"><span data-stu-id="28d9a-106">You need to have a journal mailbox and (optionally) an alternate journaling mailbox configured.</span></span> <span data-ttu-id="28d9a-107">لمعرفة المزيد، راجع ["تكوين دفتر اليومية" في Exchange Online.](https://go.microsoft.com/fwlink/?linkid=2115260)</span><span class="sxs-lookup"><span data-stu-id="28d9a-107">To learn more, see [Configure Journaling in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2115260).</span></span>
* <span data-ttu-id="28d9a-108">في Exchange Online، يوجد حد لعدد قواعد دفتر اليومية التي يمكنك إنشاؤها.</span><span class="sxs-lookup"><span data-stu-id="28d9a-108">In Exchange Online, there's a limit to the number of journal rules that you can create.</span></span> <span data-ttu-id="28d9a-109">للحصول على التفاصيل، راجع حدود قواعد دفتر [اليومية والنقل علبة الوارد.](https://go.microsoft.com/fwlink/?linkid=2115261)</span><span class="sxs-lookup"><span data-stu-id="28d9a-109">For details, see [Journal, transport, and inbox rule limits](https://go.microsoft.com/fwlink/?linkid=2115261).</span></span>
* <span data-ttu-id="28d9a-110">لا يدعم Exchange Online تسليم تقارير دفتر اليومية إلى علبة بريد Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="28d9a-110">Exchange Online doesn't support delivering journal reports to an Exchange Online mailbox.</span></span> <span data-ttu-id="28d9a-111">يجب تحديد عنوان البريد الإلكتروني لنظام أرشفة موقع أو خدمة أرشفة جهة خارجية كعميل بريد عمل اليومية.</span><span class="sxs-lookup"><span data-stu-id="28d9a-111">You must specify the email address of an on-premises archiving system or a third-party archiving service as the journaling mailbox.</span></span>
