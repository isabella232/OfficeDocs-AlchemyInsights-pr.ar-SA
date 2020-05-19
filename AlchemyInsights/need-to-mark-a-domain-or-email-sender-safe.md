---
title: هل تحتاج إلى وضع علامة على نطاق أو مرسل بريد إلكتروني آمنًا؟
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281113"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="7d70c-102">هل تحتاج إلى وضع علامة على نطاق أو مرسل بريد إلكتروني آمنًا؟</span><span class="sxs-lookup"><span data-stu-id="7d70c-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="7d70c-103">لا **يوصى باستخدام قوائم المرسلين الآمنة** نظرًا لأنه يفتح مؤسستك للهجمات غير المرغوب فيها والتصيد الاحتيالي والانتحال.</span><span class="sxs-lookup"><span data-stu-id="7d70c-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="7d70c-104">ومع ذلك، إذا كان هناك شرط عمل، **نوصي** باستخدام **[قواعد تدفق البريد](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** لهذا الغرض.</span><span class="sxs-lookup"><span data-stu-id="7d70c-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="7d70c-105">تضمن إرشاداتنا مصادقة المرسل (التحقق من عدم انتحال نطاق الإرسال).</span><span class="sxs-lookup"><span data-stu-id="7d70c-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="7d70c-106">**ملاحظة:** لا نوصي بإدارة الإيجابيات الزائفة باستخدام قوائم المرسلالآمنة، لأن الاستثناءات من تصفية الرسائل غير المرغوب فيها يمكن أن تفتح مؤسستك أمام هجمات الأمان.</span><span class="sxs-lookup"><span data-stu-id="7d70c-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="7d70c-107">إذا تلقى المستخدم (المستخدمون) رسائل تم وضع علامة غير صحيحة عليها كبريد إلكتروني غير مرغوب فيه أو غير هام، فيرجى **[الإبلاغ عن الرسائل والملفات إلى Microsoft](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="7d70c-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="7d70c-108">**يجب تجنب** المرسلين الآمنين في Outlook أو قائمة المرسل المسموح بها أو قائمة النطاقات المسموح بها في نُهج مكافحة الرسائل غير المرغوب فيها لأن المرسلين يتجاوزون جميع الرسائل غير المرغوب فيها والخداع وحماية التصيد الاحتيالي ومصادقة المرسل (SPF وDKIM وDMARC).</span><span class="sxs-lookup"><span data-stu-id="7d70c-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="7d70c-109">يتم استخدام هذا الأسلوب بشكل أفضل للاختبار المؤقت فقط.</span><span class="sxs-lookup"><span data-stu-id="7d70c-109">This method is best used for temporary testing only.</span></span>
