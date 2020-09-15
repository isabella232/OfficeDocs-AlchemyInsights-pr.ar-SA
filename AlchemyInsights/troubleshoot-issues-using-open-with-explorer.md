---
title: استكشاف الأخطاء وإصلاحها باستخدام "فتح بواسطة المستعرض"
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659045"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="42dfa-102">إصلاح المشاكل المتعلقة بالفتح باستخدام المستكشف</span><span class="sxs-lookup"><span data-stu-id="42dfa-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="42dfa-103">إصلاح المشاكل الشائعة في فتح مكتبه مستندات في SharePoint أو OneDrive باستخدام الأمر **فتح بواسطة المستعرض** :</span><span class="sxs-lookup"><span data-stu-id="42dfa-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="42dfa-104">استخدم Internet Explorer 10 أو Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="42dfa-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="42dfa-105">**الفتح باستخدام المستكشف** غير متوافق مع Microsoft Edge و Google Chrome و Firefox وغيرها.</span><span class="sxs-lookup"><span data-stu-id="42dfa-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="42dfa-106">**الفتح باستخدام المستكشف** معطل في كل المستعرضات باستثناء Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="42dfa-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="42dfa-107">لا يتوفر الخيار **فتح باستخدام المستكشف** في التجربة الحديثة لمكتبات SharePoint.</span><span class="sxs-lookup"><span data-stu-id="42dfa-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="42dfa-108">استخدم **طريقه العرض في "مستكشف الملفات** " بدلا من ذلك.</span><span class="sxs-lookup"><span data-stu-id="42dfa-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="42dfa-109">حدد طريقه عرض **خيارات** \> **العرض في "مستكشف الملفات**".</span><span class="sxs-lookup"><span data-stu-id="42dfa-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="42dfa-110">طريقه العرض في "مستكشف الملفات" غير متوافقة مع Microsoft Edge و Google Chrome و Firefox وغيرها.</span><span class="sxs-lookup"><span data-stu-id="42dfa-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="42dfa-111">تتوفر **طريقه العرض في "مستكشف الملفات** " في Internet explorer فقط.</span><span class="sxs-lookup"><span data-stu-id="42dfa-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="42dfa-112">تاكد من تشغيل خدمه WebClient.</span><span class="sxs-lookup"><span data-stu-id="42dfa-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="42dfa-113">في مربع البحث في Windows ، اكتب تشغيل ، وحدد تشغيل تطبيق سطح المكتب ، واكتب services.msc ، ثم اضغط علي مفتاح الإدخال Enter.</span><span class="sxs-lookup"><span data-stu-id="42dfa-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="42dfa-114">قم بالتمرير لأسفل وصولا إلى خدمه WebClient وتاكد من عرض عمود **الحالة** "قيد التشغيل".</span><span class="sxs-lookup"><span data-stu-id="42dfa-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="42dfa-115">إذا لم يكن الأمر كذلك ، فانقر نقرا مزدوجا فوق الخدمة ، وانقر فوق **بدء**، ثم فوق **موافق**.</span><span class="sxs-lookup"><span data-stu-id="42dfa-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="42dfa-116">(قد تحتاج إلى تمكين الخدمة أولا بتحديد اما **يدوي** أو **تلقائي** في المربع **نوع بدء التشغيل** .)</span><span class="sxs-lookup"><span data-stu-id="42dfa-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="42dfa-117">يعد فتح مكتبه في "مستكشف الملفات" مفيدا إذا كنت بحاجه إلى نسخ ملفات ومجلدات متعددة أو نقلها مره واحده ، ولكن إذا كنت تريد العمل بشكل منتظم في المكتبة ، فنوصي بمزامنتها.</span><span class="sxs-lookup"><span data-stu-id="42dfa-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="42dfa-118">لاستكشاف الأخطاء وإصلاحها في "مستكشف الملفات" ، راجع [فتح في "المستكشف"](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="42dfa-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="42dfa-119">للحصول علي معلومات حول اعداد المزامنة ، راجع [مزامنة ملفات SharePoint باستخدام عميل المزامنة من OneDrive الجديد](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="42dfa-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="42dfa-120">الرجاء مراجعه المقالة [كيفيه استخدام الأمر "فتح بواسطة المستعرض" لاستكشاف الأخطاء وإصلاحها في SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) للحصول علي مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="42dfa-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

