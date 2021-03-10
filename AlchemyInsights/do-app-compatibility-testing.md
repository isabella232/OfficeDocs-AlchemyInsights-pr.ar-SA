---
title: إجراء اختبار توافق التطبيقات
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9138"
- "9005291"
ms.openlocfilehash: 9a6a9ea3587a851ecf842588ab73421590ce2431
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692432"
---
# <a name="do-app-compatibility-testing"></a><span data-ttu-id="6c2db-102">إجراء اختبار توافق التطبيقات</span><span class="sxs-lookup"><span data-stu-id="6c2db-102">Do app compatibility testing</span></span>

<span data-ttu-id="6c2db-103">إن توافق التطبيقات ل Microsoft Edge عال جدا.</span><span class="sxs-lookup"><span data-stu-id="6c2db-103">Application compatibility for Microsoft Edge is extremely high.</span></span> <span data-ttu-id="6c2db-104">في الواقع، من العالي جدا أن توفر Microsoft وعد التوافق التالي:</span><span class="sxs-lookup"><span data-stu-id="6c2db-104">In fact, it's so high that Microsoft provides the following compatibility promises:</span></span>
- <span data-ttu-id="6c2db-105">إذا كان يعمل على Microsoft Edge 45 والإصدارات السابقة، فهو يعمل على Microsoft Edge 77 والإصدارات الأحدث.</span><span class="sxs-lookup"><span data-stu-id="6c2db-105">If it works on Microsoft Edge 45 and earlier versions, it will work on Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="6c2db-106">إذا كان يعمل على Internet Explorer، فهو يعمل على Microsoft Edge في وضع Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="6c2db-106">If it works on Internet Explorer, it will work on Microsoft Edge in Internet Explorer mode.</span></span>
- <span data-ttu-id="6c2db-107">إذا كان يعمل على Google Chrome، فهو يعمل على Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="6c2db-107">If it works on Google Chrome, it will work on Microsoft Edge.</span></span>

<span data-ttu-id="6c2db-108">إذا كان لديك تطبيق لا نلبي فيه هذا الوعود، فنحن نتحمل بعد ذلك وعدا بإصلاحه باستخدام [Microsoft App Assure.](https://www.microsoft.com/fasttrack/microsoft-365/app-assure)</span><span class="sxs-lookup"><span data-stu-id="6c2db-108">If you have an application where we don't meet this promise, then we stand behind the promise to fix it with [Microsoft App Assure](https://www.microsoft.com/fasttrack/microsoft-365/app-assure).</span></span>

<span data-ttu-id="6c2db-109">على الرغم من هذا الوعود، نحن نعلم أنه يتعين على العديد من المؤسسات التحقق من صحة بعض التطبيقات لأسباب تتعلق بالتوافق أو إدارة المخاطر.</span><span class="sxs-lookup"><span data-stu-id="6c2db-109">Despite this promise, we know that many organizations must validate some applications for compliance or risk-management reasons.</span></span> <span data-ttu-id="6c2db-110">على الرغم من توقعنا أن يكون هذا الأمر بسيطا للغاية، فمن المهم أن يتم تنظيمه وتشدد عليه في اختبار التطبيق.</span><span class="sxs-lookup"><span data-stu-id="6c2db-110">Even though we expect this to be very straightforward, it's important to be organized and rigorous in app testing.</span></span>

<span data-ttu-id="6c2db-111">هناك طريقتان للقيام باختبار توافق التطبيق:</span><span class="sxs-lookup"><span data-stu-id="6c2db-111">There are two ways to do app compatibility testing:</span></span>

- <span data-ttu-id="6c2db-112">**الاختبار** المعملي: يتم اختبار التطبيقات في بيئة تخضع لمراقبة شديدة مع تكوينات معينة.</span><span class="sxs-lookup"><span data-stu-id="6c2db-112">**Lab testing**: Applications are tested in a tightly controlled environment with specific configurations.</span></span>
- <span data-ttu-id="6c2db-113">**اختبار تجريبي:** يتم اختبار التطبيقات من قبل عدد محدود من المستخدمين في بيئة العمل اليومية الخاصة بهم باستخدام أجهزتهم الخاصة.</span><span class="sxs-lookup"><span data-stu-id="6c2db-113">**Pilot testing**: Applications are tested by a limited number of users in their daily work environment using their own devices.</span></span>

<span data-ttu-id="6c2db-114">اختر الأسلوب الأكثر ملاءمة لكل تطبيق، ثم قم باختباره قبل بدء تشغيل المؤسسة بكاملها.</span><span class="sxs-lookup"><span data-stu-id="6c2db-114">Choose the method that is most appropriate for each app and do the testing prior to a launch to the entire organization.</span></span>

<span data-ttu-id="6c2db-115">بعد التأكد من توافق تطبيقاتك، تكون جاهزا لنشر Microsoft Edge في مجموعة تجريبية.</span><span class="sxs-lookup"><span data-stu-id="6c2db-115">Once you've ensured that your apps are compatible, you're ready to deploy Microsoft Edge to a pilot group.</span></span>
