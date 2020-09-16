---
title: تشغيل تشخيص الذاكرة ل Windows في Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: f2b8306d0cd604b144b82275243c5a84580bc609
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720777"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="1c25a-102">تشغيل تشخيص الذاكرة ل Windows في Windows 10</span><span class="sxs-lookup"><span data-stu-id="1c25a-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="1c25a-103">إذا تعطل Windows والتطبيقات علي جهاز الكمبيوتر لديك أو تقوم بتجميده أو يعمل بطريقه غير مستقره ، فقد تواجه مشكله في ذاكره الكمبيوتر الشخصي (RAM).</span><span class="sxs-lookup"><span data-stu-id="1c25a-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="1c25a-104">يمكنك تشغيل تشخيص الذاكرة ل Windows للتحقق من وجود مشاكل في ذاكره الوصول العشوائي الخاصة بالكمبيوتر الشخصي.</span><span class="sxs-lookup"><span data-stu-id="1c25a-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="1c25a-105">في مربع البحث علي شريط المهام ، اكتب **تشخيص الذاكرة**، ثم حدد **تشخيص الذاكرة في Windows**.</span><span class="sxs-lookup"><span data-stu-id="1c25a-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="1c25a-106">لتشغيل التشخيص ، يجب أعاده تشغيل الكمبيوتر.</span><span class="sxs-lookup"><span data-stu-id="1c25a-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="1c25a-107">يتوفر لديك الخيار لأعاده التشغيل علي الفور (الرجاء حفظ عملك وإغلاق المستندات ورسائل البريد الكتروني المفتوحة أولا) ، أو جدوله التشخيص بحيث يتم تشغيله تلقائيا في المرة التالية التي تتم فيها أعاده تشغيل الكمبيوتر:</span><span class="sxs-lookup"><span data-stu-id="1c25a-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![تشخيص الذاكرة ل Windows](media/windows-memory-diagnostic.png)

<span data-ttu-id="1c25a-109">عند أعاده تشغيل الكمبيوتر ، سيتم تشغيل **أداه تشخيص الذاكرة في Windows** تلقائيا.</span><span class="sxs-lookup"><span data-stu-id="1c25a-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="1c25a-110">سيتم عرض الحالة والتقدم كعمليه التشخيص ، سيتوفر لديك خيار إلغاء التشخيص عن طريق القيام بالعمل علي المفتاح **ESC** علي لوحه المفاتيح.</span><span class="sxs-lookup"><span data-stu-id="1c25a-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="1c25a-111">عند اكتمال التشخيص ، سيبدا تشغيل Windows بشكل طبيعي.</span><span class="sxs-lookup"><span data-stu-id="1c25a-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="1c25a-112">بعد أعاده التشغيل مباشره ، عند ظهور سطح المكتب ، سيظهر اعلام (إلى جانب أيقونه **مركز الصيانة** علي شريط المهام) ، للاشاره إلى ما إذا تم العثور علي أخطاء في الذاكرة.</span><span class="sxs-lookup"><span data-stu-id="1c25a-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="1c25a-113">على سبيل المثال:</span><span class="sxs-lookup"><span data-stu-id="1c25a-113">For example:</span></span>

<span data-ttu-id="1c25a-114">اليك أيقونه مركز الصيانة:</span><span class="sxs-lookup"><span data-stu-id="1c25a-114">Here's the Action Center icon:</span></span> ![أيقونه مركز الصيانة](media/action-center-icon.png) 

<span data-ttu-id="1c25a-116">والاعلام النموذجي:</span><span class="sxs-lookup"><span data-stu-id="1c25a-116">And a sample notification:</span></span> ![لا توجد أخطاء في الذاكرة](media/no-memory-errors.png)

<span data-ttu-id="1c25a-118">إذا فقدت الاعلام ، يمكنك تحديد أيقونه **مركز الصيانة** علي شريط المهام لعرض **مركز الصيانة** ورؤية قائمه الإشعارات القابلة للتمرير.</span><span class="sxs-lookup"><span data-stu-id="1c25a-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="1c25a-119">لمراجعه المعلومات التفصيلية ، اكتب **حدث** في مربع البحث علي شريط المهام ، ثم حدد **عارض الاحداث**.</span><span class="sxs-lookup"><span data-stu-id="1c25a-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="1c25a-120">في الجزء الأيمن من **عارض الاحداث**، انتقل إلى **سجلات Windows > نظام**.</span><span class="sxs-lookup"><span data-stu-id="1c25a-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="1c25a-121">في الجزء الأيسر ، قم بالمسح الضوئي لأسفل في القائمة اثناء البحث في العمود **المصدر** ، حتى تري الاحداث التي تتضمن **القيمة المصدر ميموريدياجنوستيكس النتائج**.</span><span class="sxs-lookup"><span data-stu-id="1c25a-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="1c25a-122">يمكنك تمييز كل حدث والاطلاع علي معلومات النتائج في المربع ضمن علامة التبويب **عام** الموجودة أسفل القائمة.</span><span class="sxs-lookup"><span data-stu-id="1c25a-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
