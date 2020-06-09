---
title: 'خطأ: القواعد على هذا الكمبيوتر لا تتطابق'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c0982da82826d1644f437b19e0d343a59d7ac473
ms.sourcegitcommit: e09af4285c6b81ca0a5320fdb811713ac25748c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/09/2020
ms.locfileid: "44664233"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="11f3e-102">خطأ: القواعد على هذا الكمبيوتر لا تتطابق</span><span class="sxs-lookup"><span data-stu-id="11f3e-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="11f3e-103">لمشاهدة الحالة المحدثة لهذه المشكلة المعروفة، راجع [القواعد على هذا الكمبيوتر لا تتطابق مع القواعد على Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="11f3e-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="11f3e-104">قام فريق Outlook بتنفيذ إصلاح في بناء 12928.10000.</span><span class="sxs-lookup"><span data-stu-id="11f3e-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="11f3e-105">الإصلاح هو بالفعل في منالداخل السريع وسوف تذهب إلى القناة الشهرية في أواخر يونيو 2020.</span><span class="sxs-lookup"><span data-stu-id="11f3e-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="11f3e-106">وبمجرد الانتهاء من بناء ثابت قد تحصل على موجه "القواعد التي تريد الاحتفاظ بها" مرة أخيرة.</span><span class="sxs-lookup"><span data-stu-id="11f3e-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="11f3e-107">اختر الخادم عند المطالبة ثم العودة في Outlook وإعادة تمكين أي قواعد تم تعطيلها.</span><span class="sxs-lookup"><span data-stu-id="11f3e-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="11f3e-108">حتى يتوفر الإصلاح الرجاء استخدام الحل البديل التالي:</span><span class="sxs-lookup"><span data-stu-id="11f3e-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="11f3e-109">**الحل البديل:** في التقارير الأخيرة، حدثت المشكلة لتلك التي أنشأت قواعد العميل فقط في سطح مكتب Outlook.</span><span class="sxs-lookup"><span data-stu-id="11f3e-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="11f3e-110">إذا كنت لا تزال تواجه المشكلة، خذ بعين الاعتبار حذف القواعد ثم إنشاء القواعد وتحريرها فقط في OWA (Outlook Web App) حتى يتم حل المشكلة.</span><span class="sxs-lookup"><span data-stu-id="11f3e-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="11f3e-111">إذا لم تتمكن من حذف القواعد يدوياً يمكنك تشغيل أمر Outlook عند بدء تشغيل Outlook عن طريق تشغيل Outlook.exe /cleanrules.</span><span class="sxs-lookup"><span data-stu-id="11f3e-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="11f3e-112">سيؤدي ذلك إلى حذف كل من قواعد العميل والملقم.</span><span class="sxs-lookup"><span data-stu-id="11f3e-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="11f3e-113">فإنه سيتم حذف كافة القواعد لكافة الحسابات في ملف تعريف Outlook.</span><span class="sxs-lookup"><span data-stu-id="11f3e-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="11f3e-114">يتم توثيق هذا الأمر في مقالة مفاتيح سطر الأوامر.</span><span class="sxs-lookup"><span data-stu-id="11f3e-114">This command is further documented in the Command-line switches article.</span></span>

