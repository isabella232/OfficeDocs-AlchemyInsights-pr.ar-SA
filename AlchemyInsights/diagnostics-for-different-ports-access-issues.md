---
title: تشخيص مشاكل الوصول إلى المنافذ المختلفة
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51034748"
---
# <a name="diagnostics-for-different-ports-access-issues"></a><span data-ttu-id="18bd7-102">تشخيص مشاكل الوصول إلى المنافذ المختلفة</span><span class="sxs-lookup"><span data-stu-id="18bd7-102">Diagnostics for different ports access issues</span></span>

<span data-ttu-id="18bd7-103">لحل المشاكل المختلفة المتعلقة بالوصول إلى المنفذ، يمكنك تنفيذ الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="18bd7-103">To resolve the different port access issues, perform the following steps:</span></span>

1. <span data-ttu-id="18bd7-104">توقف/deallocate الجهاز الظاهري (VM) من المدخل، ثم أعد تشغيل VM، ثم اختبر مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="18bd7-104">Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span></span> 
2. <span data-ttu-id="18bd7-105">تحقق من إعدادات شبكة VM لتحديد ما إذا كان لديك مجموعات أمان الشبكة (NSG) تمنع حركة المرور.</span><span class="sxs-lookup"><span data-stu-id="18bd7-105">Check your VM's network settings to determine if you have Network Security Groups (NSGs) blocking traffic.</span></span> <span data-ttu-id="18bd7-106">يمكنك أيضا استخدام أداة التحقق من تدفق [IP](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) الخاصة بمراقب الشبكة للتحقق من حظر NSGs لحركة المرور، أو توجيه User-Defined (UDRs) لإعادة توجيه حركة المرور إلى المحلية ('المسار الافتراضي' 0.0.0/0) أو إلى جهاز شبكة.</span><span class="sxs-lookup"><span data-stu-id="18bd7-106">You can also use [Network Watcher's IP flow verify tool](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) to check for NSGs blocking traffic, User-Defined Routes (UDRs) rerouting your traffic back to on-premises ('Default Route' 0.0.0.0/0), or to a network appliance.</span></span>
<span data-ttu-id="18bd7-107">إذا ما زلت تواجه مشاكل بعد تجربة الخطوات المذكورة أعلاه، فالرجاء توفير اسم VM وميناء TCP الذي تحاول إرسال البريد عليه لإجراء المزيد من التشخيصات.</span><span class="sxs-lookup"><span data-stu-id="18bd7-107">If you still experience issues after trying the steps above, please provide the VM name and the TCP port you are attempting to send mail on for further diagnosis.</span></span>

<span data-ttu-id="18bd7-108">**المستندات المستحسنة**</span><span class="sxs-lookup"><span data-stu-id="18bd7-108">**Recommended Documents**</span></span>

[<span data-ttu-id="18bd7-109">القيود والتوصيات المتعلقة بإرسال البريد الإلكتروني الصادر عبر المنفذ 25</span><span class="sxs-lookup"><span data-stu-id="18bd7-109">Limitations and recommendations for sending outbound email over port 25</span></span>](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)