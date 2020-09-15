---
title: 'الخطا: القواعد الموجودة علي هذا الكمبيوتر غير متطابقة'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690950"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="993ee-102">الخطا: القواعد الموجودة علي هذا الكمبيوتر غير متطابقة</span><span class="sxs-lookup"><span data-stu-id="993ee-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="993ee-103">للاطلاع علي الحالة المحدثة لهذه المشكلة المعروفة ، راجع [القواعد الموجودة علي هذا الكمبيوتر لا تتطابق مع قواعد Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="993ee-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="993ee-104">قام فريق Outlook بتطبيق تصحيح في الإصدار 12928.10000.</span><span class="sxs-lookup"><span data-stu-id="993ee-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="993ee-105">التصحيح موجود بالفعل في Insider سينتقل إلى القناة الشهرية في يونيو 2020 المتاخر.</span><span class="sxs-lookup"><span data-stu-id="993ee-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="993ee-106">بمجرد ان تحصل علي البنية الثابتة ، يمكنك الحصول علي القاعدة التي تريد الاحتفاظ بها في المرة الواحدة الاخيره.</span><span class="sxs-lookup"><span data-stu-id="993ee-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="993ee-107">اختر خادم عند مطالبتك بذلك ، ثم عد إلى Outlook ثم أعد تمكين اي قواعد تم تعطيلها.</span><span class="sxs-lookup"><span data-stu-id="993ee-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="993ee-108">حتى يتوفر التصحيح الرجاء استخدام الحل البديل التالي:</span><span class="sxs-lookup"><span data-stu-id="993ee-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="993ee-109">**الحل البديل**: في التقارير الاخيره ، حدثت المشكلة للأشخاص الذين لديهم قواعد عميل تم إنشاؤها فقط في Outlook لسطح المكتب.</span><span class="sxs-lookup"><span data-stu-id="993ee-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="993ee-110">إذا استمرت المشكلة ، فيمكنك حذف القواعد ثم إنشاء القواعد وتحريرها فقط في OWA (Outlook Web App) حتى يتم حل المشكلة.</span><span class="sxs-lookup"><span data-stu-id="993ee-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="993ee-111">إذا لم تتمكن من حذف القواعد يدويا ، فيمكنك تشغيل أمر Outlook عند بدء تشغيل Outlook بتشغيل Outlook.exe/cleanrules.</span><span class="sxs-lookup"><span data-stu-id="993ee-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="993ee-112">سيؤدي هذا إلى حذف قواعد العميل والخادم.</span><span class="sxs-lookup"><span data-stu-id="993ee-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="993ee-113">سيؤدي هذا إلى حذف كل القواعد لكل الحسابات في ملف تعريف Outlook.</span><span class="sxs-lookup"><span data-stu-id="993ee-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="993ee-114">هذا الأمر موثق بشكل أكبر في المقالة رموز التبديل في سطر الأوامر.</span><span class="sxs-lookup"><span data-stu-id="993ee-114">This command is further documented in the Command-line switches article.</span></span>

