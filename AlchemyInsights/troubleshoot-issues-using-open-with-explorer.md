---
title: استكشاف أخطاء وإصلاحها باستخدام فتح باستخدام مستكشف
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 03bb3ad01a716390ec50845b29ddf6cc81a83116
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/22/2019
ms.locfileid: "30759281"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="8951f-102">إصلاح المشاكل المتعلقة بفتح باستخدام مستكشف</span><span class="sxs-lookup"><span data-stu-id="8951f-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="8951f-103">إصلاح المشاكل الشائعة المتعلقة بفتح مكتبة مستندات SharePoint أو أونيدريفي باستخدام الأمر **فتح بواسطة المستعرض** :</span><span class="sxs-lookup"><span data-stu-id="8951f-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="8951f-104">استخدام Internet Explorer 10 أو 11 من برنامج Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="8951f-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="8951f-105">**فتح باستخدام مستكشف** غير متوافق مع Microsoft الحافة، جوجل كروم، فايرفوكس وغيرها.</span><span class="sxs-lookup"><span data-stu-id="8951f-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="8951f-106">**فتح باستخدام "مستكشف"** معطل في كافة المستعرضات استثناء Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="8951f-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="8951f-107">**فتح باستخدام "مستكشف"** غير متوفر في التجربة الحديثة لمكتبات SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8951f-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="8951f-108">استخدم **طريقة عرض في "مستكشف الملفات"** بدلاً من ذلك.</span><span class="sxs-lookup"><span data-stu-id="8951f-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="8951f-109">حدد **خيارات العرض** \> **طريقة عرض في "مستكشف الملفات"**.</span><span class="sxs-lookup"><span data-stu-id="8951f-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="8951f-110">طريقة عرض في "مستكشف الملفات" غير متوافق مع Microsoft الحافة، جوجل كروم، فايرفوكس وغيرها.</span><span class="sxs-lookup"><span data-stu-id="8951f-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="8951f-111">**طريقة عرض في "مستكشف الملفات"** في متوفر فقط في Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="8951f-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="8951f-112">تأكد من تشغيل خدمة WebClient.</span><span class="sxs-lookup"><span data-stu-id="8951f-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="8951f-113">في المربع بحث Windows، نوع التشغيل، حدد سطح المكتب تشغيل التطبيق ثم اكتب services.msc وثم اضغط Enter.</span><span class="sxs-lookup"><span data-stu-id="8951f-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="8951f-114">قم بالتمرير لأسفل إلى خدمة WebClient وتأكد من أن يعرض عمود **الحالة** "قيد التشغيل".</span><span class="sxs-lookup"><span data-stu-id="8951f-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="8951f-115">إذا لم يكن كذلك، انقر نقراً مزدوجاً فوق الخدمة، انقر فوق **ابدأ**، وثم انقر فوق **موافق**.</span><span class="sxs-lookup"><span data-stu-id="8951f-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="8951f-116">(قد تحتاج إلى تمكين الخدمة أولاً بتحديد أما **يدوياً** أو **تلقائياً** في المربع **نوع بدء التشغيل** ).</span><span class="sxs-lookup"><span data-stu-id="8951f-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="8951f-117">فتح مكتبة في "مستكشف الملفات" مفيد إذا كنت تريد نسخ أو نقل ملفات ومجلدات متعددة مرة واحدة، ولكن إذا كنت تريد أن تعمل بشكل منتظم في المكتبة، نوصي بمزامنته.</span><span class="sxs-lookup"><span data-stu-id="8951f-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="8951f-118">استكشاف أخطاء مشاكل فتح "مستكشف الملفات"، راجع [فتح في مستكشف](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="8951f-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="8951f-119">للحصول على مزيد من المعلومات حول إعداد المزامنة، راجع [الملفات SharePoint متزامنة مع عميل المزامنة أونيدريفي الجديد](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="8951f-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="8951f-120">الرجاء مراجعة المقالة [كيفية استخدام الأمر "فتح باستخدام" مستكشف "" لاستكشاف مشاكل في SharePoint عبر إنترنت](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="8951f-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) for more information.</span></span> 
  

