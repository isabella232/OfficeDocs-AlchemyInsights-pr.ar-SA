---
title: استخدام موقع ويب Wix مع المجالات التي تم شراؤها أو مداره من Microsoft
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/05/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5855"
- "9003096"
ms.openlocfilehash: f6845c56f05e9cef11362ce601a974b73a154c9a
ms.sourcegitcommit: 28a319e482e6a8644e87726e1b0e599819df52d0
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2020
ms.locfileid: "46629332"
---
# <a name="using-a-wix-website-with-microsoft-purchased-or-managed-domains"></a><span data-ttu-id="a82dd-102">استخدام موقع ويب Wix مع المجالات التي تم شراؤها أو مداره من Microsoft</span><span class="sxs-lookup"><span data-stu-id="a82dd-102">Using a Wix website with Microsoft purchased or managed domains</span></span>

<span data-ttu-id="a82dd-103">للحصول علي معلومات حول كيفيه استخدام موقع ويب Wix مع مجال تم شراؤه أو مدار من قبل Microsoft ، راجع [تحديث سجلات DNS للاحتفاظ بموقعك علي ويب مع موفر الاستضافة الحالي](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider).</span><span class="sxs-lookup"><span data-stu-id="a82dd-103">For information about how to use a Wix website with a Microsoft purchased or managed domain, see [Update DNS records to keep your website with your current hosting provider](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider).</span></span>

<span data-ttu-id="a82dd-104">للحصول علي التفاصيل ، راجع:</span><span class="sxs-lookup"><span data-stu-id="a82dd-104">For details, see:</span></span> 

- <span data-ttu-id="a82dd-105">Wix المقالة "الاتصال بمجال إلى Wix باستخدام أسلوب التاشير ،" يوصي باضافه سجلات DNS كما هو مبين في الارتباط أعلاه بدلا من تغيير خوادم الأسماء عند استخدام Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a82dd-105">The Wix article, "Connecting a Domain to Wix Using the Pointing Method," recommends adding DNS records as outlined in the link above rather than changing names servers when you're using Microsoft 365.</span></span>

- <span data-ttu-id="a82dd-106">إذا اخترت تغيير خوادم الأسماء إلى Wix ، فيجب إنشاء سجلات DNS في Wix لشركه Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a82dd-106">If you choose to change name servers to Wix, you must create DNS records at Wix for Microsoft.</span></span> <span data-ttu-id="a82dd-107">لمزيد من المعلومات ، راجع [إنشاء سجلات DNS في Wix ل Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix).</span><span class="sxs-lookup"><span data-stu-id="a82dd-107">For more info, see [Create DNS records at Wix for Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix).</span></span>

- <span data-ttu-id="a82dd-108">إذا تم شراء مجالك من Microsoft ، فلا يمكن تغيير خوادم الأسماء.</span><span class="sxs-lookup"><span data-stu-id="a82dd-108">If your domain was purchased from Microsoft the name servers can't be changed.</span></span> <span data-ttu-id="a82dd-109">إذا كان يجب عليك تغيير خوادم الأسماء ، فيجب نقل المجال الذي اشتريته Microsoft إلى موفر استضافه آخر بعد 60 يوما.</span><span class="sxs-lookup"><span data-stu-id="a82dd-109">If you must change names servers, the Microsoft purchased domain must be transferred to another hosting provider after 60 days.</span></span> <span data-ttu-id="a82dd-110">لمزيد من المعلومات ، راجع [الاسئله المتداولة حول المجالات](https://docs.microsoft.com/microsoft-365/admin/setup/domains-faq#can-i-transfer-a-domain-i-purchased-from-microsoft-to-another-provider).</span><span class="sxs-lookup"><span data-stu-id="a82dd-110">For more info, see the [Domains FAQ](https://docs.microsoft.com/microsoft-365/admin/setup/domains-faq#can-i-transfer-a-domain-i-purchased-from-microsoft-to-another-provider).</span></span>