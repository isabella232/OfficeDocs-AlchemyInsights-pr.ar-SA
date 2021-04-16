---
title: يؤدي النقر نقرا مزدوجا فوق ملف Office إلى فشل فتحه
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: b9c563f7dd099bf3bad9018f69e2096816dd7290
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814792"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="b983e-102">يؤدي النقر نقرا مزدوجا فوق ملف Office إلى فشل فتحه</span><span class="sxs-lookup"><span data-stu-id="b983e-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="b983e-103">بعد النقر نقرا مزدوجا فوق ملف Office، قد ترى البرنامج مفتوحا ولكن الملف نفسه لا يفتح.</span><span class="sxs-lookup"><span data-stu-id="b983e-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="b983e-104">أو قد تحصل على رسالة الخطأ: "كانت هناك مشكلة في إرسال الأمر إلى البرنامج".</span><span class="sxs-lookup"><span data-stu-id="b983e-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="b983e-105">ثمة أسباب كثيرة وراء ذلك، ولكن الحلين الأكثر شيوعا هو:</span><span class="sxs-lookup"><span data-stu-id="b983e-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="b983e-106">من داخل Excel، تأكد من إلغاء تحديد خيار DDE.</span><span class="sxs-lookup"><span data-stu-id="b983e-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="b983e-107">يمكن العثور على الخيار عن طريق إنشاء مصنف جديد ثم اختيار ملف > خيارات > **متقدمة.**</span><span class="sxs-lookup"><span data-stu-id="b983e-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="b983e-108">في المقطع **عام،** أ إلغاء تحديد تجاهل التطبيقات الأخرى التي تستخدم تبادل البيانات الديناميكي **(DDE)**.</span><span class="sxs-lookup"><span data-stu-id="b983e-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="b983e-109">تشغيل إصلاح عبر الإنترنت لاستعادة الإعدادات الافتراضية.</span><span class="sxs-lookup"><span data-stu-id="b983e-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="b983e-110">انقر فوق زر البدء في Windows وابحث عن "لوحة التحكم".</span><span class="sxs-lookup"><span data-stu-id="b983e-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="b983e-111">افتح **لوحة التحكم**، واذهب إلى البرامج > **والبرامج والميزات**.</span><span class="sxs-lookup"><span data-stu-id="b983e-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="b983e-112">ثم انقر ب زر الماوس الأيمن فوق **Microsoft Office [الإصدار]** **واختر تغيير**> عبر الإنترنت .</span><span class="sxs-lookup"><span data-stu-id="b983e-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="b983e-113">إذا لم ينجح أي من هذين الحلين، يمكن العثور على قائمة حلول أكثر اكتمالا في مقالة الدعم، يؤدي النقر المزدوج فوق ملف Office إلى فشل [فتحه.](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)</span><span class="sxs-lookup"><span data-stu-id="b983e-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
