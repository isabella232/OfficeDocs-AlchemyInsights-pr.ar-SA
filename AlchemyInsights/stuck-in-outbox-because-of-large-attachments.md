---
title: عالقة في علبة الصادر بسبب مرفقات كبيرة
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
- "9002385"
- "4645"
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241239"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="41732-102">إصلاح الرسائل العالقة في علبة الصادر</span><span class="sxs-lookup"><span data-stu-id="41732-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="41732-103">نوصي بالبدء بتشغيل السيناريو ["أواجه مشاكل في إرسال رسائل البريد الإلكتروني أو تلقيها أو العثور عليها"](https://aka.ms/SaRA-OutlookSendReceive) من أداة [مساعد دعم واسترداد Microsoft.](https://diagnostics.office.com/#/)</span><span class="sxs-lookup"><span data-stu-id="41732-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="41732-104">عندما تتعثر رسالة في علبة الصادر، السبب الأكثر احتمالاً هو مرفق كبير أو الخيار "إرسال فوراً عند الاتصال" غير ممكّن.</span><span class="sxs-lookup"><span data-stu-id="41732-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="41732-105">**إزالة المرفق الكبير**</span><span class="sxs-lookup"><span data-stu-id="41732-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="41732-106">في Outlook، حدد **إرسال / تلقي** > **العمل دون اتصال**.</span><span class="sxs-lookup"><span data-stu-id="41732-106">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="41732-107">في جزء التنقل، حدد **علبة الصادر**.</span><span class="sxs-lookup"><span data-stu-id="41732-107">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="41732-108">من هنا، يمكنك:</span><span class="sxs-lookup"><span data-stu-id="41732-108">From here, you can:</span></span> 
    - <span data-ttu-id="41732-109">حذف الرسالة (حددها ثم حدد **حذف**).</span><span class="sxs-lookup"><span data-stu-id="41732-109">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="41732-110">اسحب الرسالة إلى مجلد المسودات، وانقر نقرًا مزدوجًا لفتحها، وإزالة المرفق حددها ثم حدد **حذف**).</span><span class="sxs-lookup"><span data-stu-id="41732-110">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="41732-111">إذا تلقيت خطأ يقول Outlook يحاول إرسال الرسالة إغلاق Outlook.</span><span class="sxs-lookup"><span data-stu-id="41732-111">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="41732-112">قد يستغرق الأمر بضع لحظات للخروج.</span><span class="sxs-lookup"><span data-stu-id="41732-112">It may take a few moments to exit.</span></span> <span data-ttu-id="41732-113">إذا لم يتم إغلاق Outlook، اضغط على Ctrl+Alt+Delete وحدد **بدء إدارة المهام**.</span><span class="sxs-lookup"><span data-stu-id="41732-113">If Outlook doesn't close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="41732-114">في إدارة المهام، حدد علامة التبويب **العمليات،** ومرر لأسفل إلى outlook.exe، وحدد **عملية النهاية**.</span><span class="sxs-lookup"><span data-stu-id="41732-114">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="41732-115">بعد إغلاق Outlook، أعد تشغيله وكرر الخطوتين 2 و3.</span><span class="sxs-lookup"><span data-stu-id="41732-115">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="41732-116">بعد إزالة المرفق، انقر فوق **إرسال / تلقي** > **العمل دون اتصال** لاستئناف العمل عبر الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="41732-116">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="41732-117">تتعثر الرسائل أيضًا في علبة الصادر عند النقر فوق **إرسال**، ولكنك غير متصل.</span><span class="sxs-lookup"><span data-stu-id="41732-117">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="41732-118">انقر فوق **إرسال / تلقي** وإلقاء نظرة على زر العمل دون **اتصال.**</span><span class="sxs-lookup"><span data-stu-id="41732-118">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="41732-119">إذا كان أزرق، فأنت مفصول.</span><span class="sxs-lookup"><span data-stu-id="41732-119">If it's blue, you're disconnected.</span></span> <span data-ttu-id="41732-120">انقر فوقه للاتصال (يتحول الزر إلى اللون الأبيض) وانقر فوق **إرسال الكل**.</span><span class="sxs-lookup"><span data-stu-id="41732-120">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="41732-121">**تمكين الإرسال على الفور عند الاتصال**</span><span class="sxs-lookup"><span data-stu-id="41732-121">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="41732-122">في علامة التبويب "ملف"، انقر فوق **الخيارات**.</span><span class="sxs-lookup"><span data-stu-id="41732-122">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="41732-123">في مربع حوار خيارات Outlook، انقر فوق **متقدم**.</span><span class="sxs-lookup"><span data-stu-id="41732-123">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="41732-124">في قسم الإرسال والاستقبال، انقر لتمكين **الإرسال على الفور عند الاتصال**.</span><span class="sxs-lookup"><span data-stu-id="41732-124">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="41732-125">انقر فوق **موافق**.</span><span class="sxs-lookup"><span data-stu-id="41732-125">Click **OK**.</span></span>
 
<span data-ttu-id="41732-126">للحصول على التفاصيل الكاملة، انظر:</span><span class="sxs-lookup"><span data-stu-id="41732-126">For full details, see:</span></span>
- [<span data-ttu-id="41732-127">فيديو: إرسال بريد إلكتروني عالق أو حذفه</span><span class="sxs-lookup"><span data-stu-id="41732-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="41732-128">يبقى البريد الإلكتروني في مجلد علبة الصادر حتى تبدأ عملية إرسال/استقبال يدويًا في Outlook</span><span class="sxs-lookup"><span data-stu-id="41732-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
