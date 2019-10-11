---
title: عالقه في علبه الصادر بسبب المرفقات الكبيرة
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
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441293"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="9df1e-102">إصلاح الرسائل التي عالقه في علبه الصادر</span><span class="sxs-lookup"><span data-stu-id="9df1e-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="9df1e-103">من المستحسن ان تبدا بتشغيل السيناريو ["أواجه مشاكل في إرسال رسائل البريد الكتروني أو تلقيها أو العثور](https://aka.ms/SaRA-OutlookSendReceive) عليها" من أداه [دعم Microsoft ومساعد الاسترداد](https://diagnostics.office.com/#/) .</span><span class="sxs-lookup"><span data-stu-id="9df1e-103">We recommend that you start by running the scenario ["I’m having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="9df1e-104">عندما يعلق رسالة في علبه الصادر ، الأسباب الأكثر احتمالا:</span><span class="sxs-lookup"><span data-stu-id="9df1e-104">When a message gets stuck in your Outbox, the most likely causes are:</span></span>
- <span data-ttu-id="9df1e-105">ملحقات كبيره.</span><span class="sxs-lookup"><span data-stu-id="9df1e-105">Large attachments.</span></span>
- <span data-ttu-id="9df1e-106">لم يتم تمكين الخيار **إرسال فورا عند الاتصال** .</span><span class="sxs-lookup"><span data-stu-id="9df1e-106">The **Send immediately when connected** option is not enabled.</span></span>

<span data-ttu-id="9df1e-107">لأزاله المرفقات الكبيرة:</span><span class="sxs-lookup"><span data-stu-id="9df1e-107">To remove large attachments:</span></span> 

1. <span data-ttu-id="9df1e-108">في Outlook ، حدد **إرسال/تلقي** > **العمل دون اتصال**.</span><span class="sxs-lookup"><span data-stu-id="9df1e-108">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="9df1e-109">في جزء التنقل ، حدد **علبه الصادر**.</span><span class="sxs-lookup"><span data-stu-id="9df1e-109">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="9df1e-110">من هنا ، يمكنك:</span><span class="sxs-lookup"><span data-stu-id="9df1e-110">From here, you can:</span></span> 
    - <span data-ttu-id="9df1e-111">احذف الرسالة (حددها ثم حدد **حذف**).</span><span class="sxs-lookup"><span data-stu-id="9df1e-111">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="9df1e-112">اسحب الرسالة إلى مجلد "المسودات" ، وانقر نقرا مزدوجا لفتحه ، وقم بازاله المرفق حدده ثم حدد **حذف**).</span><span class="sxs-lookup"><span data-stu-id="9df1e-112">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="9df1e-113">إذا تلقيت خطا يقول Outlook يحاول إرسال الرسالة ، اغلق Outlook.</span><span class="sxs-lookup"><span data-stu-id="9df1e-113">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="9df1e-114">قد يستغرق الأمر بضع لحظات للخروج.</span><span class="sxs-lookup"><span data-stu-id="9df1e-114">It may take a few moments to exit.</span></span> <span data-ttu-id="9df1e-115">إذا لم يتم إغلاق Outlook ، اضغط Ctrl + Alt + Delete وحدد **بدء تشغيل أداره المهام**.</span><span class="sxs-lookup"><span data-stu-id="9df1e-115">If Outlook doesn’t close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="9df1e-116">في "أداره المهام" ، حدد علامة التبويب **العمليات** ، قم بالتمرير لأسفل إلى outlook ، ثم حدد **إنهاء العملية**.</span><span class="sxs-lookup"><span data-stu-id="9df1e-116">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="9df1e-117">بعد إغلاق Outlook ، أعد تشغيله وكرر الخطوتين 2 و 3.</span><span class="sxs-lookup"><span data-stu-id="9df1e-117">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="9df1e-118">بعد أزاله المرفق ، انقر فوق **إرسال/تلقي** > **العمل دون اتصال** لاستئناف العمل عبر الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="9df1e-118">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="9df1e-119">الرسائل أيضا الحصول علي عالقه في علبه الصادر عند النقر فوق **إرسال**ولكن لم تكن متصلا.</span><span class="sxs-lookup"><span data-stu-id="9df1e-119">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="9df1e-120">انقر فوق **إرسال/تلقي** وإلقاء نظره علي **العمل دون اتصال** زر.</span><span class="sxs-lookup"><span data-stu-id="9df1e-120">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="9df1e-121">إذا كان ازرق ، فأنت مفصول.</span><span class="sxs-lookup"><span data-stu-id="9df1e-121">If it's blue, you're disconnected.</span></span> <span data-ttu-id="9df1e-122">حدده للاتصال (الزر يتحول إلى اللون الأبيض) وانقر علي **إرسال الكل**.</span><span class="sxs-lookup"><span data-stu-id="9df1e-122">Select it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="9df1e-123">لتمكين **الإرسال فورا عند الاتصال**:</span><span class="sxs-lookup"><span data-stu-id="9df1e-123">To enable **Send immediately when connected**:</span></span>
 
- <span data-ttu-id="9df1e-124">حدد**خيارات** >   **الملف** > **المتقدمة**.</span><span class="sxs-lookup"><span data-stu-id="9df1e-124">Select **File** > **Options** >  **Advanced**.</span></span>
<span data-ttu-id="9df1e-125">في المقطع **إرسال وتلقي** ، حدد **إرسال فورا عند الاتصال**، ثم اختر **موافق**.</span><span class="sxs-lookup"><span data-stu-id="9df1e-125">In the **Send and receive** section, select **Send immediately when connected**, and then choose **OK**.</span></span>
 
<span data-ttu-id="9df1e-126">للاطلاع علي التفاصيل الكاملة ، انظر:</span><span class="sxs-lookup"><span data-stu-id="9df1e-126">For full details see:</span></span>
- [<span data-ttu-id="9df1e-127">فيديو: إرسال بريد الكتروني عالق أو حذفه</span><span class="sxs-lookup"><span data-stu-id="9df1e-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="9df1e-128">يبقي البريد الكتروني في المجلد "علبه الصادر" حتى تقوم يدويا ببدء عمليه إرسال/تلقي في Outlook</span><span class="sxs-lookup"><span data-stu-id="9df1e-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
