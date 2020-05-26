---
title: تشغيل تشخيص ذاكرة Windows في Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/19/2020
ms.locfileid: "44357249"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="ffb29-102">تشغيل تشخيص ذاكرة Windows في Windows 10</span><span class="sxs-lookup"><span data-stu-id="ffb29-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="ffb29-103">إذا تعطلت النوافذ والتطبيقات الموجودة على الكمبيوتر أو تجمدها أو تتصرف بطريقة غير مستقرة، فقد تواجه مشكلة في ذاكرة الكمبيوتر (RAM).</span><span class="sxs-lookup"><span data-stu-id="ffb29-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="ffb29-104">يمكنك تشغيل تشخيص ذاكرة Windows للتحقق من وجود مشاكل في ذاكرة الوصول العشوائي للكمبيوتر.</span><span class="sxs-lookup"><span data-stu-id="ffb29-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="ffb29-105">في مربع البحث على شريط المهام، اكتب **تشخيص الذاكرة،** ثم حدد **تشخيص ذاكرة Windows**.</span><span class="sxs-lookup"><span data-stu-id="ffb29-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="ffb29-106">لتشغيل التشخيص، يحتاج الكمبيوتر إلى إعادة التشغيل.</span><span class="sxs-lookup"><span data-stu-id="ffb29-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="ffb29-107">لديك خيار إعادة التشغيل على الفور (الرجاء حفظ عملك وإغلاق المستندات المفتوحة ورسائل البريد الإلكتروني أولاً)، أو جدولة التشخيص لتشغيله تلقائيًا في المرة التالية التي يتم فيها إعادة تشغيل الكمبيوتر:</span><span class="sxs-lookup"><span data-stu-id="ffb29-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![تشخيص ذاكرة Windows](media/windows-memory-diagnostic.png)

<span data-ttu-id="ffb29-109">عند إعادة تشغيل الكمبيوتر، سيتم تشغيل **أداة تشخيص ذاكرة Windows** تلقائيًا.</span><span class="sxs-lookup"><span data-stu-id="ffb29-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="ffb29-110">سيتم عرض الحالة والتقدم أثناء تشغيل التشخيص، ولديك خيار إلغاء التشخيص عن طريق الضغط على مفتاح **ESC** على لوحة المفاتيح.</span><span class="sxs-lookup"><span data-stu-id="ffb29-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="ffb29-111">عند اكتمال التشخيص، سيبدأ Windows بشكل طبيعي.</span><span class="sxs-lookup"><span data-stu-id="ffb29-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="ffb29-112">مباشرة بعد إعادة التشغيل، عند ظهور سطح المكتب، سيظهر إعلام (بجوار رمز **مركز الإجراءات** على شريط المهام)، للإشارة إلى ما إذا كان قد تم العثور على أية أخطاء في الذاكرة.</span><span class="sxs-lookup"><span data-stu-id="ffb29-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="ffb29-113">على سبيل المثال:</span><span class="sxs-lookup"><span data-stu-id="ffb29-113">For example:</span></span>

<span data-ttu-id="ffb29-114">إليك رمز مركز الإجراءات:</span><span class="sxs-lookup"><span data-stu-id="ffb29-114">Here's the Action Center icon:</span></span> ![أيقونة مركز الإجراءات](media/action-center-icon.png) 

<span data-ttu-id="ffb29-116">وعينة إعلام:</span><span class="sxs-lookup"><span data-stu-id="ffb29-116">And a sample notification:</span></span> ![لا توجد أخطاء في الذاكرة](media/no-memory-errors.png)

<span data-ttu-id="ffb29-118">إذا فاتك الإعلام، يمكنك تحديد رمز **مركز الإجراءات** على شريط المهام لعرض **مركز الإجراءات** ومشاهدة قائمة إعلامات قابلة للتمرير.</span><span class="sxs-lookup"><span data-stu-id="ffb29-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="ffb29-119">لمراجعة المعلومات التفصيلية، اكتب **الحدث** في مربع البحث على شريط المهام، ثم حدد **عارض الأحداث**.</span><span class="sxs-lookup"><span data-stu-id="ffb29-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="ffb29-120">في الجزء الأيسر **لعارض الأحداث،** انتقل إلى **Windows Logs > System**.</span><span class="sxs-lookup"><span data-stu-id="ffb29-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="ffb29-121">في الجزء الأيمن، قم بمسح القائمة أثناء النظر إلى عمود **المصدر،** حتى ترى الأحداث ذات القيمة المصدر **MemoryDiagnostics-Results**.</span><span class="sxs-lookup"><span data-stu-id="ffb29-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="ffb29-122">قم بتمييز كل حدث من هذا القبيل وراجع معلومات النتيجة في المربع أسفل علامة التبويب **العامة** أسفل القائمة.</span><span class="sxs-lookup"><span data-stu-id="ffb29-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
