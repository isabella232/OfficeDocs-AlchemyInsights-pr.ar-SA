---
title: تشغيل تشخيص الذاكرة في Windows في Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826654"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="1c73a-102">تشغيل تشخيص الذاكرة في Windows في Windows 10</span><span class="sxs-lookup"><span data-stu-id="1c73a-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="1c73a-103">إذا تعطلت تطبيقات Windows وتطبيقات على الكمبيوتر الشخصي أو تجمدت أو تصرفت بطريقة غير مستقرة، فقد تواجه مشكلة في ذاكرة الكمبيوتر (RAM).</span><span class="sxs-lookup"><span data-stu-id="1c73a-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="1c73a-104">يمكنك تشغيل تشخيص الذاكرة ل Windows للتحقق من مشاكل ذاكرة الوصول العشوائي للكمبيوتر الشخصي.</span><span class="sxs-lookup"><span data-stu-id="1c73a-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="1c73a-105">في مربع البحث على شريط المهام، اكتب **تشخيص الذاكرة**، ثم حدد Windows **Memory Diagnostic**.</span><span class="sxs-lookup"><span data-stu-id="1c73a-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="1c73a-106">لتشغيل التشخيص، يجب إعادة تشغيل الكمبيوتر.</span><span class="sxs-lookup"><span data-stu-id="1c73a-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="1c73a-107">لديك خيار إعادة التشغيل على الفور (الرجاء حفظ عملك وأغلق المستندات المفتوحة والبريد الإلكتروني أولا)، أو قم لجدولة التشخيص ليعمل تلقائيا في المرة التالية التي يقوم فيها الكمبيوتر بإعادة تشغيل:</span><span class="sxs-lookup"><span data-stu-id="1c73a-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![تشخيص الذاكرة في Windows](media/windows-memory-diagnostic.png)

<span data-ttu-id="1c73a-109">عند إعادة تشغيل الكمبيوتر الشخصي، سيتم تشغيل أداة تشخيص الذاكرة ل **Windows** تلقائيا.</span><span class="sxs-lookup"><span data-stu-id="1c73a-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="1c73a-110">سيتم عرض الحالة والتقدم عند تشغيل التشخيص، وسيبقى لديك خيار إلغاء التشخيصات عن طريق الضغط على المفتاح **ESC** على لوحة المفاتيح.</span><span class="sxs-lookup"><span data-stu-id="1c73a-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="1c73a-111">عند اكتمال التشخيص، سيبدأ Windows بشكل طبيعي.</span><span class="sxs-lookup"><span data-stu-id="1c73a-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="1c73a-112">بعد إعادة التشغيل مباشرة، عندما يظهر سطح المكتب، سيظهر إعلام (بجانب أيقونة **مركز** الإجراءات على شريط المهام)، للإشارة إلى ما إذا تم العثور على أي أخطاء في الذاكرة.</span><span class="sxs-lookup"><span data-stu-id="1c73a-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="1c73a-113">على سبيل المثال:</span><span class="sxs-lookup"><span data-stu-id="1c73a-113">For example:</span></span>

<span data-ttu-id="1c73a-114">فيما يلي أيقونة مركز الإجراءات:</span><span class="sxs-lookup"><span data-stu-id="1c73a-114">Here's the Action Center icon:</span></span> ![أيقونة مركز الإجراءات](media/action-center-icon.png) 

<span data-ttu-id="1c73a-116">ونموذج إعلام:</span><span class="sxs-lookup"><span data-stu-id="1c73a-116">And a sample notification:</span></span> ![لا توجد أخطاء في الذاكرة](media/no-memory-errors.png)

<span data-ttu-id="1c73a-118">إذا فاتك الإعلام، يمكنك تحديد  أيقونة مركز الإجراءات على  شريط المهام لعرض مركز الإجراءات لمشاهدة قائمة قابلة للتمرير من الإعلامات.</span><span class="sxs-lookup"><span data-stu-id="1c73a-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="1c73a-119">لمراجعة المعلومات المفصلة، **اكتب** حدثا في مربع البحث على شريط المهام، ثم حدد **عارض الأحداث**.</span><span class="sxs-lookup"><span data-stu-id="1c73a-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="1c73a-120">في **الجزء** الأيسر من عارض الأحداث، انتقل إلى **سجلات Windows > System**.</span><span class="sxs-lookup"><span data-stu-id="1c73a-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="1c73a-121">في الجزء الأيسر، قم بفحص القائمة لأسفل أثناء  النظر إلى العمود المصدر، حتى ترى الأحداث باستخدام **القيمة المصدر MemoryDiagnostics-Results**.</span><span class="sxs-lookup"><span data-stu-id="1c73a-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="1c73a-122">يمكنك تمييز كل حدث من هذا النوع لمشاهدة معلومات النتائج في المربع ضمن علامة **التبويب عام** أسفل القائمة.</span><span class="sxs-lookup"><span data-stu-id="1c73a-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
