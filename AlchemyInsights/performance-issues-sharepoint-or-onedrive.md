---
title: مشاكل الأداء-SharePoint أو OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771888"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="4685c-102">SharePoint أو OneDrive البطيء أو القابل للوصول أو غير متوفر لعده مستخدمين</span><span class="sxs-lookup"><span data-stu-id="4685c-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="4685c-103">قد يكون SharePoint أو OneDrive بطيئا أو لا يمكن الوصول اليه أو غير متاح ، أو قد يعرض الخدمة غير متوفرة أو أخطاء 503 ، لأسباب عديده:</span><span class="sxs-lookup"><span data-stu-id="4685c-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="4685c-104">إذا كان موقع SharePoint أو OneDrive بطيئا أو متاخرا لعده مستخدمين ، فقد يكون هناك مشكله خدمه مؤقته حيث يواجه المستخدمون تاخيرات متقطعه أو أخطاء في التنقل عند الوصول إلى مواقع SharePoint أو محتوي OneDrive.</span><span class="sxs-lookup"><span data-stu-id="4685c-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="4685c-105">راجع [لوحه معلومات حماية الخدمة](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) لمعرفه ما إذا كانت مؤسستك متاثره بالأمر.</span><span class="sxs-lookup"><span data-stu-id="4685c-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="4685c-106">قد يتلقى المستخدمون خطا في *503 الخادم* عند محاولة الانتقال إلى مواقع SharePoint أو OneDrive.</span><span class="sxs-lookup"><span data-stu-id="4685c-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="4685c-107">قد يعود سبب هذا الخطا إلى التحكم في خدمه SharePoint.</span><span class="sxs-lookup"><span data-stu-id="4685c-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="4685c-108">يستخدم SharePoint Online التقييد للمحافظة على الأداء الأمثل وإمكانية الاعتماد على خدمة SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="4685c-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="4685c-109">يحد التقييد من عدد إجراءات المستخدم أو المكالمات المتزامنة (بواسطة البرنامج النصي أو التعليمات البرمجية) لمنع الاستخدام المفرط للموارد.</span><span class="sxs-lookup"><span data-stu-id="4685c-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="4685c-110">للحصول علي مزيد من المعلومات حول التحكم ، يمكنك [تجنب الوصول إلى SharePoint Online أو حظره](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="4685c-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="4685c-111">إذا كنت تواجه بطء في الأداء باستخدام موقع أو صفحه SharePoint **التقليدية** أو **الحديثة** ، فيمكنك استخدام [أداه تشخيص الصفحة](https://aka.ms/perftool) لتحليل الصفحات.</span><span class="sxs-lookup"><span data-stu-id="4685c-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="4685c-112">إذا كنت لا تزال تواجه الأداء البطيء بشكل عام ، فالرجاء مراجعه الموارد في أسفل هذه المقالة: [مقدمه حول توليف الأداء ل SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="4685c-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  