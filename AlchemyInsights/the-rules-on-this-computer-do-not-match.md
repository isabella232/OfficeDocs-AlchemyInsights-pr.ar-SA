---
title: 'خطأ: القواعد على هذا الكمبيوتر غير متطابقة'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782939"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="3539f-102">خطأ: القواعد على هذا الكمبيوتر غير متطابقة</span><span class="sxs-lookup"><span data-stu-id="3539f-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="3539f-103">لرؤية الحالة المحدثة لهذه المشكلة المعروفة، راجع القواعد على هذا الكمبيوتر لا تتطابق [مع القواعد في Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="3539f-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="3539f-104">نفذ فريق Outlook تصحيحا في البنية 12928.10000.</span><span class="sxs-lookup"><span data-stu-id="3539f-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="3539f-105">الإصلاح موجود بالفعل في Insider Fast وسيذهب إلى القناة الشهرية في أواخر يونيو 2020.</span><span class="sxs-lookup"><span data-stu-id="3539f-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="3539f-106">بمجرد الحصول على البنية الثابتة، قد تحصل على المطالبة "ما هي القواعد التي تريد الاحتفاظ بها" مرة واحدة أخيرة.</span><span class="sxs-lookup"><span data-stu-id="3539f-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="3539f-107">اختر الخادم عند مطالبتك بذلك، ثم ارجع إلى Outlook ثم اعاد تمكين أي قواعد تم تعطيلها.</span><span class="sxs-lookup"><span data-stu-id="3539f-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="3539f-108">حتى يتوفر الإصلاح، الرجاء استخدام الحل البديل التالي:</span><span class="sxs-lookup"><span data-stu-id="3539f-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="3539f-109">**الحل البديل**: في التقارير الأخيرة، حدثت المشكلة لهؤلاء الذين أنشأوا قواعد العميل فقط في Outlook لسطح المكتب.</span><span class="sxs-lookup"><span data-stu-id="3539f-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="3539f-110">إذا استمرت المشكلة، فنظر في حذف القواعد ثم قم بإنشاء القواعد وتحريرها فقط في OWA (Outlook Web App) حتى يتم حل المشكلة.</span><span class="sxs-lookup"><span data-stu-id="3539f-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="3539f-111">إذا لم تتمكن من حذف القواعد يدويا، يمكنك تشغيل أمر Outlook عند بدء تشغيل Outlook عن طريق تشغيل Outlook.exe /cleanrules.</span><span class="sxs-lookup"><span data-stu-id="3539f-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="3539f-112">سيحذف هذا كلا من قواعد العميل وخادم.</span><span class="sxs-lookup"><span data-stu-id="3539f-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="3539f-113">سيتم حذف كل القواعد لكل الحسابات في ملف تعريف Outlook.</span><span class="sxs-lookup"><span data-stu-id="3539f-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="3539f-114">تم توثيق هذا الأمر بشكل أكبر في مقالة تبديل سطر الأوامر.</span><span class="sxs-lookup"><span data-stu-id="3539f-114">This command is further documented in the Command-line switches article.</span></span>

