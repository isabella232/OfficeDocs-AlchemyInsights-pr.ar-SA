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
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232617"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="de257-102">إصلاح الرسائل العالقة في علبة الصادر</span><span class="sxs-lookup"><span data-stu-id="de257-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="de257-103">نوصي بالبدء بتشغيل السيناريو ["أواجه مشاكل في إرسال رسائل البريد الإلكتروني أو تلقيها أو العثور عليها"](https://aka.ms/SaRA-OutlookSendReceive) من أداة [مساعد دعم واسترداد Microsoft](https://diagnostics.office.com/#/) على الجهاز المتأثر.</span><span class="sxs-lookup"><span data-stu-id="de257-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool on the affected machine.</span></span>

<span data-ttu-id="de257-104">عندما تتعثر رسالة في علبة الصادر، السبب الأكثر احتمالاً هو مرفق كبير أو الخيار "إرسال فوراً عند الاتصال" غير ممكّن.</span><span class="sxs-lookup"><span data-stu-id="de257-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="de257-105">**إزالة المرفق الكبير**</span><span class="sxs-lookup"><span data-stu-id="de257-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="de257-106">انقر فوق **إرسال / تلقي** > **العمل دون اتصال**.</span><span class="sxs-lookup"><span data-stu-id="de257-106">Click **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="de257-107">في جزء التنقل، انقر فوق **علبة الصادر**.</span><span class="sxs-lookup"><span data-stu-id="de257-107">In the navigation pane, click **Outbox**.</span></span> <span data-ttu-id="de257-108">من هنا، يمكنك:</span><span class="sxs-lookup"><span data-stu-id="de257-108">From here, you can:</span></span> 
    - <span data-ttu-id="de257-109">حذف الرسالة.</span><span class="sxs-lookup"><span data-stu-id="de257-109">Delete the message.</span></span> <span data-ttu-id="de257-110">ما عليك سوى تحديده وانقر فوق **حذف**.</span><span class="sxs-lookup"><span data-stu-id="de257-110">Just select it and click **Delete**.</span></span>
    - <span data-ttu-id="de257-111">اسحب الرسالة إلى **مجلد المسودات،** وانقر نقراً مزدوجاً لفتح الرسالة، وحذف المرفق (انقر فوقه وانقر فوق **حذف**).</span><span class="sxs-lookup"><span data-stu-id="de257-111">Drag the message to your **drafts folder**, double-click to open the message, and delete the attachment (click it and click **Delete**).</span></span>
3. <span data-ttu-id="de257-112">إذا كان خطأ يخبرك Outlook يحاول إرسال الرسالة إغلاق Outlook.</span><span class="sxs-lookup"><span data-stu-id="de257-112">If an error tells you Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="de257-113">قد يستغرق الأمر بضع لحظات للخروج.</span><span class="sxs-lookup"><span data-stu-id="de257-113">It may take a few moments to exit.</span></span> <span data-ttu-id="de257-114">إذا لم يتم إغلاق Outlook، اضغط **على Ctrl+Alt+Delete** وانقر فوق **بدء إدارة المهام**.</span><span class="sxs-lookup"><span data-stu-id="de257-114">If Outlook doesn't close, press **Ctrl+Alt+Delete** and click **Start Task Manager**.</span></span> <span data-ttu-id="de257-115">في إدارة المهام، حدد علامة التبويب **العمليات،** ومرر لأسفل إلى outlook.exe، وانقر فوق **إنهاء العملية**.</span><span class="sxs-lookup"><span data-stu-id="de257-115">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and click **End Process**.</span></span>
4. <span data-ttu-id="de257-116">بعد إغلاق Outlook، إعادة تشغيل Outlook وتكرار الخطوات 2-3.</span><span class="sxs-lookup"><span data-stu-id="de257-116">After Outlook closes, restart Outlook and repeat steps 2-3.</span></span> 
5. <span data-ttu-id="de257-117">بعد إزالة المرفق، انقر فوق **إرسال / تلقي** > **العمل دون اتصال** لإلغاء تحديد الزر واستئناف العمل عبر الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="de257-117">After you remove the attachment, click **Send / Receive** > **Work Offline** to deselect the button and to resume working online.</span></span> 

<span data-ttu-id="de257-118">تتعثر الرسائل أيضًا في علبة الصادر عند النقر فوق **إرسال**، ولكنك غير متصل.</span><span class="sxs-lookup"><span data-stu-id="de257-118">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="de257-119">انقر فوق **إرسال / تلقي** وإلقاء نظرة على زر العمل دون **اتصال.**</span><span class="sxs-lookup"><span data-stu-id="de257-119">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="de257-120">إذا كان أزرق، فأنت مفصول.</span><span class="sxs-lookup"><span data-stu-id="de257-120">If it's blue, you're disconnected.</span></span> <span data-ttu-id="de257-121">انقر فوقه للاتصال (يتحول الزر إلى اللون الأبيض) وانقر فوق **إرسال الكل**.</span><span class="sxs-lookup"><span data-stu-id="de257-121">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="de257-122">**تمكين الإرسال على الفور عند الاتصال**</span><span class="sxs-lookup"><span data-stu-id="de257-122">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="de257-123">في علامة التبويب "ملف"، انقر فوق **الخيارات**.</span><span class="sxs-lookup"><span data-stu-id="de257-123">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="de257-124">في مربع حوار خيارات Outlook، انقر فوق **متقدم**.</span><span class="sxs-lookup"><span data-stu-id="de257-124">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="de257-125">في قسم الإرسال والاستقبال، انقر لتمكين **الإرسال على الفور عند الاتصال**.</span><span class="sxs-lookup"><span data-stu-id="de257-125">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="de257-126">انقر فوق **موافق**.</span><span class="sxs-lookup"><span data-stu-id="de257-126">Click **OK**.</span></span>
 
<span data-ttu-id="de257-127">للحصول على التفاصيل الكاملة، انظر:</span><span class="sxs-lookup"><span data-stu-id="de257-127">For full details, see:</span></span>
- [<span data-ttu-id="de257-128">فيديو: إرسال بريد إلكتروني عالق أو حذفه</span><span class="sxs-lookup"><span data-stu-id="de257-128">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="de257-129">يبقى البريد الإلكتروني في مجلد علبة الصادر حتى تبدأ عملية إرسال/استقبال يدويًا في Outlook</span><span class="sxs-lookup"><span data-stu-id="de257-129">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
