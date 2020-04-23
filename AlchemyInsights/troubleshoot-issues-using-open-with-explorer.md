---
title: استكشاف المشاكل وإصلاحها باستخدام فتح مع Explorer
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: cb26876d93a110b3b0addd7821206215c783f959
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759679"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="c83f4-102">إصلاح المشاكل مع فتح مع مستكشف</span><span class="sxs-lookup"><span data-stu-id="c83f4-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="c83f4-103">إصلاح المشاكل الشائعة في فتح مكتبة مستندات في SharePoint أو OneDrive باستخدام الأمر **فتح مع Explorer:**</span><span class="sxs-lookup"><span data-stu-id="c83f4-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="c83f4-104">استخدم إنترنت إكسبلورر 10 أو إنترنت إكسبلورر 11.</span><span class="sxs-lookup"><span data-stu-id="c83f4-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="c83f4-105">**فتح مع إكسبلورر** غير متوافق مع مايكروسوفت إيدج وجوجل كروم وفايرفوكس وغيرها.</span><span class="sxs-lookup"><span data-stu-id="c83f4-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="c83f4-106">**تم** تعطيل فتح مع Explorer في جميع المتصفحات باستثناء Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="c83f4-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="c83f4-107">**فتح مع إكسبلورر** غير متوفر في التجربة الحديثة لمكتبات SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c83f4-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="c83f4-108">استخدم **طريقة العرض في مستكشف الملفات** بدلاً من ذلك.</span><span class="sxs-lookup"><span data-stu-id="c83f4-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="c83f4-109">حدد **عرض خيارات** \> **العرض في مستكشف الملفات**.</span><span class="sxs-lookup"><span data-stu-id="c83f4-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="c83f4-110">عرض في ملف إكسبلورر غير متوافق مع مايكروسوفت إيدج، جوجل كروم، فايرفوكس وغيرها.</span><span class="sxs-lookup"><span data-stu-id="c83f4-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="c83f4-111">**عرض في مستكشف الملفات** في متوفر فقط في Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="c83f4-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="c83f4-112">تأكد من تشغيل خدمة WebClient.</span><span class="sxs-lookup"><span data-stu-id="c83f4-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="c83f4-113">في مربع بحث Windows، اكتب التشغيل، وحدد تطبيق تشغيل سطح المكتب، واكتب services.msc، ثم اضغط على إدخال.</span><span class="sxs-lookup"><span data-stu-id="c83f4-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="c83f4-114">مرر لأسفل إلى خدمة WebClient وتأكد من عرض عمود **الحالة** "قيد التشغيل".</span><span class="sxs-lookup"><span data-stu-id="c83f4-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="c83f4-115">إذا لم يكن كذلك، انقر نقراً مزدوجاً على الخدمة، انقر فوق **ابدأ،** ثم انقر فوق **موافق**.</span><span class="sxs-lookup"><span data-stu-id="c83f4-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="c83f4-116">(قد تحتاج أولاً إلى تمكين الخدمة عن طريق تحديد **إما يدوي** أو **تلقائي** في مربع نوع **بدء التشغيل.)**</span><span class="sxs-lookup"><span data-stu-id="c83f4-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="c83f4-117">يعد فتح مكتبة في File Explorer مفيدًا إذا كنت بحاجة إلى نسخ ملفات ومجلدات متعددة أو نقلها مرة واحدة ، ولكن إذا كنت ترغب في العمل بانتظام في المكتبة ، فإننا نوصي بمزامنتها.</span><span class="sxs-lookup"><span data-stu-id="c83f4-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="c83f4-118">لاستكشاف المشاكل التي يتم فتحها في مستكشف الملفات، راجع [فتح في Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="c83f4-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="c83f4-119">للحصول على معلومات حول إعداد المزامنة، راجع [ملفات مزامنة SharePoint مع عميل مزامنة OneDrive الجديد](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="c83f4-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="c83f4-120">الرجاء الاطلاع على المقالة [كيفية استخدام الأمر "فتح مع مستكشف" لاستكشاف المشكلات في SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) لمزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="c83f4-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

