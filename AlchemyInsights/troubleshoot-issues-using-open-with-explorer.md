---
title: استكشاف أخطاء وإصلاحها باستخدام فتح باستخدام مستكشف
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: c95f07b9fb7251442577c014e4005dbe3f92ceb4
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/30/2019
ms.locfileid: "29661738"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="077de-102">إصلاح المشاكل المتعلقة بفتح باستخدام مستكشف</span><span class="sxs-lookup"><span data-stu-id="077de-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="077de-103">إصلاح المشاكل الشائعة المتعلقة بفتح مكتبة مستندات SharePoint أو أندريف باستخدام الأمر **فتح بواسطة المستعرض** :</span><span class="sxs-lookup"><span data-stu-id="077de-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="077de-p101">استخدام Internet Explorer 10 أو 11 من برنامج Internet Explorer. **فتح باستخدام مستكشف** غير متوافق مع Microsoft الحافة، جوجل كروم، فايرفوكس وغيرها. **فتح باستخدام "مستكشف"** معطل في كافة المستعرضات استثناء Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="077de-p101">Use Internet Explorer 10 or Internet Explorer 11. **Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others. **Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="077de-p102">**فتح باستخدام "مستكشف"** غير متوفر في التجربة الحديثة لمكتبات SharePoint. استخدم **طريقة عرض في "مستكشف الملفات"** بدلاً من ذلك. حدد **خيارات العرض** \> **طريقة عرض في "مستكشف الملفات"**. طريقة عرض في "مستكشف الملفات" غير متوافق مع Microsoft الحافة، جوجل كروم، فايرفوكس وغيرها. **طريقة عرض في "مستكشف الملفات"** في متوفر فقط في Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="077de-p102">**Open with Explorer** is not available in the modern experience for SharePoint libraries. Use **View in File Explorer** instead. Select **View options** \> **View in File Explorer**. View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others. **View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="077de-p103">تأكد من تشغيل خدمة WebClient. في المربع بحث Windows، نوع التشغيل، حدد سطح المكتب تشغيل التطبيق ثم اكتب services.msc وثم اضغط Enter. قم بالتمرير لأسفل إلى خدمة WebClient وتأكد من أن يعرض عمود **الحالة** "قيد التشغيل". إذا لم يكن كذلك، انقر نقراً مزدوجاً فوق الخدمة، انقر فوق **ابدأ**، وثم انقر فوق **موافق**. (قد تحتاج إلى تمكين الخدمة أولاً بتحديد أما **يدوياً** أو **تلقائياً** في المربع **نوع بدء التشغيل** ).</span><span class="sxs-lookup"><span data-stu-id="077de-p103">Make sure the WebClient service is running. In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter. Scroll down to the WebClient service and make sure the **Status** column displays "Running." If it doesn't, double-click the service, click **Start**, and then click **OK**. (You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="077de-p104">فتح مكتبة في "مستكشف الملفات" مفيد إذا كنت تريد نسخ أو نقل ملفات ومجلدات متعددة مرة واحدة، ولكن إذا كنت تريد أن تعمل بشكل منتظم في المكتبة، نوصي بمزامنته. استكشاف أخطاء مشاكل فتح "مستكشف الملفات"، راجع [فتح في مستكشف](https://go.microsoft.com/fwlink/?linkid=871665). للحصول على مزيد من المعلومات حول إعداد المزامنة، راجع [الملفات SharePoint متزامنة مع عميل المزامنة أندريف الجديد](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="077de-p104">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it. To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="077de-120">الرجاء مراجعة المقالة [كيفية استخدام الأمر "فتح باستخدام" مستكشف "" لاستكشاف مشاكل في SharePoint عبر إنترنت](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="077de-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) for more information.</span></span> 
  

