---
title: استخدام DLP في قواعد النقل
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: 124b031e2e029b745c66a71f681f57134739eafe
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915006"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="8b66d-102">استخدام DLP في قواعد النقل</span><span class="sxs-lookup"><span data-stu-id="8b66d-102">Using DLP in transport rules</span></span>

<span data-ttu-id="8b66d-103">لدمج تفادي فقدان البيانات (DLP) في عملية نقل موجودة، استخدم الشرط "**إذا كانت الرسالة تحتوي على...المعلومات الحساسة**" في إعداد قاعدة النقل.</span><span class="sxs-lookup"><span data-stu-id="8b66d-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="8b66d-104">**لمزيد من التفاصيل، اطلع على:**</span><span class="sxs-lookup"><span data-stu-id="8b66d-104">**For more details, see:**</span></span>

- <span data-ttu-id="8b66d-105">أنواع المعلومات الحساسة لتقنية DLP المتكاملة في قواعد النقل: [تكامل قواعد المعلومات الحساسة](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="8b66d-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="8b66d-106">يمكنك أيضاً اختبار القاعدة باستخدام اختبار النهج أو بدونه باستخدام "وضع الاختبار" على القاعدة.</span><span class="sxs-lookup"><span data-stu-id="8b66d-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="8b66d-107">يجب الانتظار 30 دقيقة بعد إنشاء القاعدة قبل اختبارها.</span><span class="sxs-lookup"><span data-stu-id="8b66d-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="8b66d-108">راجع [اختبار قواعد تدفق/نقل البريد](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="8b66d-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="8b66d-109">**ملاحظة**: إذا كنت تحاول تنفيذ نهج DLP جديد باستخدام قواعد النقل في EAC، فاستخدم [نهج DLP في مركز التوافق والأمان](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) بدلاً من ذلك.</span><span class="sxs-lookup"><span data-stu-id="8b66d-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
