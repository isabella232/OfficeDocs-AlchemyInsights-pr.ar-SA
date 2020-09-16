---
title: استرداد العناصر المحذوفة باستخدام cmdlet
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
- "1800008"
- "5718"
ms.openlocfilehash: 91a9bcf75b13881b903a1d3b6f2da53f65811c9c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741290"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="ebc70-102">استرداد العناصر المحذوفة باستخدام cmdlet</span><span class="sxs-lookup"><span data-stu-id="ebc70-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="ebc70-103">استخدم الأمر [ريكوفيرابليتيمس](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet لعرض العناصر المحذوفة في علب البريد.</span><span class="sxs-lookup"><span data-stu-id="ebc70-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="ebc70-104">بعد العثور علي العناصر المحذوفة ، يمكنك استخدام [ريكوفيرابليتيمس](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet لاستعادتها.</span><span class="sxs-lookup"><span data-stu-id="ebc70-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="ebc70-105">اطلع [علي التفاصيل الكاملة في ريكوفيرابليتيمس](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="ebc70-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="ebc70-106">يجب ان يتم تعيين دور تصدير "استيراد علبه البريد" قبل ان تتمكن من تشغيل أمر cmdlet هذا.</span><span class="sxs-lookup"><span data-stu-id="ebc70-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="ebc70-107">يرجى الاطلاع علي [ريكوفيرابليتيمس](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) للحصول علي مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="ebc70-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
