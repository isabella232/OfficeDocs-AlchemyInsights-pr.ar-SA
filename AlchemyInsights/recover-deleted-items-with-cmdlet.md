---
title: استرداد العناصر المحذوفة باستخدام cmdlet
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
- "1800008"
- "5718"
ms.openlocfilehash: d8f2a50f39d7bcd321692ab093e2efa6613e9814
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835798"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="1b13c-102">استرداد العناصر المحذوفة باستخدام cmdlet</span><span class="sxs-lookup"><span data-stu-id="1b13c-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="1b13c-103">استخدم [الأمر Cmdlet Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) لعرض العناصر المحذوفة في علب البريد.</span><span class="sxs-lookup"><span data-stu-id="1b13c-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="1b13c-104">بعد العثور على العناصر المحذوفة، يمكنك استخدام [الأمر cmdlet Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) لاستعادتها.</span><span class="sxs-lookup"><span data-stu-id="1b13c-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="1b13c-105">راجع التفاصيل الكاملة في [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="1b13c-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="1b13c-106">يجب تعيين دور استيراد تصدير علبة البريد قبل أن تتمكن من تشغيل الأمر cmdlet هذا.</span><span class="sxs-lookup"><span data-stu-id="1b13c-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="1b13c-107">الرجاء الاطلاع [على Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="1b13c-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
