---
title: فتح باستخدام مستكشف لا يعمل
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
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 7680766b53bd5e85789375d3f9e9ab635780ec6c
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538444"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="b0108-102">فتح باستخدام مستكشف لا يعمل</span><span class="sxs-lookup"><span data-stu-id="b0108-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="b0108-103">إذا لم يعمل على **فتح باستخدام "مستكشف"** أو **طريقة عرض في "مستكشف الملفات"** تأكد من تعيين **تشغيل** خدمة WebClient باتباع الخطوات التالية.</span><span class="sxs-lookup"><span data-stu-id="b0108-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="b0108-104">على سبيل المثال، قد يستغرق وقتاً طويلاً لفتح مكتبة SharePoint أو أندريف عند عدم تشغيل الخدمة.</span><span class="sxs-lookup"><span data-stu-id="b0108-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="b0108-105">في مربع "البحث في Windows"، تشغيل نوع، حدد تطبيق سطح المكتب تشغيل ونوع services.msc ثم حدد **Enter**.</span><span class="sxs-lookup"><span data-stu-id="b0108-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="b0108-106">قم بالتمرير لأسفل إلى خدمة WebClient والتحقق من عمود **الحالة** .</span><span class="sxs-lookup"><span data-stu-id="b0108-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="b0108-107">إذا حالة خدمة WebClient ليست **قيد التشغيل**، انقر نقراً مزدوجاً فوق الخدمة، انقر فوق **ابدأ**، وثم انقر فوق **موافق**.</span><span class="sxs-lookup"><span data-stu-id="b0108-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="b0108-108">تمكين الخدمة، إذا لزم الأمر، عن طريق تحديد **يدوي** أو **تلقائي** في المربع **نوع بدء التشغيل** .</span><span class="sxs-lookup"><span data-stu-id="b0108-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="b0108-109">استكشاف أخطاء مشاكل فتح "مستكشف الملفات"، راجع [فتح في مستكشف](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="b0108-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="b0108-110">استكشاف المزامنة كبديل أفضل: [الملفات SharePoint متزامنة مع عميل المزامنة أندريف الجديد](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="b0108-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

