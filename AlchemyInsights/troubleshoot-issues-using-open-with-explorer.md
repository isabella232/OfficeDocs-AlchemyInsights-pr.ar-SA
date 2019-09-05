---
title: استكشاف المشكلات وإصلاحها باستخدام فتح باستخدام Explorer
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
ms.openlocfilehash: a9ab7dd27e4dc1bd76c93cc81260616063e638ed
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742720"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="bbc83-102">إصلاح المشاكل مع فتح مع مستكشف</span><span class="sxs-lookup"><span data-stu-id="bbc83-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="bbc83-103">إصلاح المشكلات الشائعة حول فتح مكتبة مستندات في SharePoint أو أندريف باستخدام الأمر **فتح باستخدام** مستكشف:</span><span class="sxs-lookup"><span data-stu-id="bbc83-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="bbc83-104">استخدام Internet Explorer 10 أو Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="bbc83-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="bbc83-105">**فتح مع إكسبلورر** غير متوافق مع مايكروسوفت إيدج، جوجل كروم، فايرفوكس وغيرها.</span><span class="sxs-lookup"><span data-stu-id="bbc83-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="bbc83-106">**فتح مع مستكشف** مع تعطيل في كافة المستعرضات باستثناء Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="bbc83-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="bbc83-107">**فتح مع مستكشف** غير متوفر في التجربة الحديثة لمكتبات SharePoint.</span><span class="sxs-lookup"><span data-stu-id="bbc83-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="bbc83-108">استخدام **طريقة العرض في "مستكشف الملفات"** بدلاً من ذلك.</span><span class="sxs-lookup"><span data-stu-id="bbc83-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="bbc83-109">حدد **عرض خيارات** \> **العرض في مستكشف الملفات**.</span><span class="sxs-lookup"><span data-stu-id="bbc83-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="bbc83-110">عرض في مستكشف الملفات غير متوافق مع مايكروسوفت إيدج، جوجل كروم، فايرفوكس وغيرها.</span><span class="sxs-lookup"><span data-stu-id="bbc83-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="bbc83-111">**عرض في مستكشف الملفات** في متوفر فقط في Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="bbc83-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="bbc83-112">تأكد من تشغيل خدمة WebClient.</span><span class="sxs-lookup"><span data-stu-id="bbc83-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="bbc83-113">في مربع البحث في Windows، اكتب تشغيل، حدد تشغيل تطبيق سطح المكتب، اكتب services.msc، ثم اضغط Enter.</span><span class="sxs-lookup"><span data-stu-id="bbc83-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="bbc83-114">قم بالتمرير لأسفل إلى خدمة WebClient وتأكد من عرض عمود **الحالة** "قيد التشغيل".</span><span class="sxs-lookup"><span data-stu-id="bbc83-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="bbc83-115">إذا لم يكن كذلك، انقر نقراً مزدوجاً فوق الخدمة، وانقر فوق **ابدأ**، ثم انقر فوق **موافق**.</span><span class="sxs-lookup"><span data-stu-id="bbc83-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="bbc83-116">(قد تحتاج أولاً إلى تمكين الخدمة عن طريق تحديد **إما يدوي** أو **تلقائي** في المربع نوع **بدء التشغيل.)**</span><span class="sxs-lookup"><span data-stu-id="bbc83-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="bbc83-117">فتح مكتبة في مستكشف الملفات مفيد إذا كنت بحاجة إلى نسخ أو نقل ملفات ومجلدات متعددة مرة واحدة، ولكن إذا كنت ترغب في العمل بانتظام في المكتبة، نوصي بمزامنتها.</span><span class="sxs-lookup"><span data-stu-id="bbc83-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="bbc83-118">لاستكشاف المشكلات التي يتم فتحها في مستكشف الملفات وإصلاحها، راجع [فتح في Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="bbc83-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="bbc83-119">للحصول على معلومات حول إعداد المزامنة، راجع [مزامنة ملفات SharePoint مع عميل المزامنة OneDrive الجديد](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="bbc83-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="bbc83-120">الرجاء مراجعة المقالة [كيفية استخدام الأمر "فتح باستخدام مستكشف" لاستكشاف المشكلات في SharePoint على الإنترنت](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="bbc83-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

