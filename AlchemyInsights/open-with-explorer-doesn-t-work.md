---
title: فتح مع مستكشف لا يعمل
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
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713021"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="8eca1-102">فتح مع مستكشف لا يعمل</span><span class="sxs-lookup"><span data-stu-id="8eca1-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="8eca1-103">إذا **كان فتح مع مستكشف** أو عرض في مستكشف **الملفات** لا يعمل تأكد من تعيين خدمة WebClient إلى **قيد التشغيل** باتباع الخطوات التالية.</span><span class="sxs-lookup"><span data-stu-id="8eca1-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="8eca1-104">على سبيل المثال، قد يستغرق وقتاً طويلاً لفتح مكتبة SharePoint أو OneDrive عند عدم تشغيل الخدمة.</span><span class="sxs-lookup"><span data-stu-id="8eca1-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="8eca1-105">في مربع بحث Windows، اكتب التشغيل، وحدد تطبيق تشغيل سطح المكتب، واكتب services.msc، ثم حدد **إدخال**.</span><span class="sxs-lookup"><span data-stu-id="8eca1-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="8eca1-106">مرر لأسفل إلى خدمة WebClient وتحقق من **عمود الحالة.**</span><span class="sxs-lookup"><span data-stu-id="8eca1-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="8eca1-107">إذا لم تكن حالة خدمة WebClient **قيد التشغيل**، انقر نقرًا مزدوجًا على الخدمة ، انقر فوق **ابدأ**، ثم انقر فوق **موافق**.</span><span class="sxs-lookup"><span data-stu-id="8eca1-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="8eca1-108">تمكين الخدمة، إذا لزم الأمر، عن طريق تحديد **إما يدوي** أو **تلقائي** في مربع نوع **بدء التشغيل.**</span><span class="sxs-lookup"><span data-stu-id="8eca1-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="8eca1-109">لاستكشاف المشاكل التي يتم فتحها في مستكشف الملفات، راجع [فتح في Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="8eca1-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="8eca1-110">استكشاف المزامنة كبديل أفضل: [مزامنة ملفات SharePoint مع عميل مزامنة OneDrive الجديد](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="8eca1-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

