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
ms.openlocfilehash: 07c108d5292965d20340da039b67744d93c0a4fc61edb8115796671f2f7f1552
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030889"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>تشخيص مشاكل الوصول إلى المنافذ المختلفة

لحل المشاكل المختلفة المتعلقة بالوصول إلى المنفذ، يمكنك تنفيذ الخطوات التالية:

1. توقف/deallocate الجهاز الظاهري (VM) من المدخل، ثم أعد تشغيل VM، ثم اختبر مرة أخرى. 
2. تحقق من إعدادات شبكة VM لتحديد ما إذا كان لديك مجموعات أمان الشبكة (NSG) تمنع حركة المرور. يمكنك أيضا استخدام أداة التحقق من تدفق [IP](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) الخاصة بمراقب الشبكة للتحقق من حظر NSGs لحركة المرور، أو توجيه User-Defined (UDRs) لإعادة توجيه حركة المرور إلى المحلية ('المسار الافتراضي' 0.0.0/0) أو إلى جهاز شبكة.
إذا ما زلت تواجه مشاكل بعد تجربة الخطوات المذكورة أعلاه، فالرجاء توفير اسم VM وميناء TCP الذي تحاول إرسال البريد عليه لإجراء المزيد من التشخيصات.

**المستندات الموصى بها**

[القيود والتوصيات المتعلقة بإرسال البريد الإلكتروني الصادر عبر المنفذ 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)