---
title: مشكلات الأداء-SharePoint أو اندريف
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068373"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="5fc1d-102">SharePoint أو اندريف بطيئه أو غير قابله للوصول أو غير متوفرة لعده مستخدمين</span><span class="sxs-lookup"><span data-stu-id="5fc1d-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="5fc1d-103">قد يكون SharePoint أو OneDrive بطيئا أو غير قابل للوصول أو غير متوفر أو قد يعرض الخدمة غير متوفرة أو أخطاء 503 لعده أسباب:</span><span class="sxs-lookup"><span data-stu-id="5fc1d-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="5fc1d-104">إذا كان موقع SharePoint أو OneDrive الخاص بك بطيئا أو مؤجلا لعده مستخدمين ، قد تكون هناك مشكله خدمه مؤقته حيث يواجه المستخدمون تاخيرات متقطعه أو أخطاء في التنقل عند الوصول إلى مواقع SharePoint أو محتوي OneDrive.</span><span class="sxs-lookup"><span data-stu-id="5fc1d-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="5fc1d-105">تحقق من [لوحه معلومات صحة الخدمة](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) لمعرفه ما إذا كانت مؤسستك قد تاثرت.</span><span class="sxs-lookup"><span data-stu-id="5fc1d-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="5fc1d-106">قد يتلقى المستخدمون *ملقم 503 هو خطا مشغول* عند محاولة الانتقال إلى مواقع SharePoint أو اندريف.</span><span class="sxs-lookup"><span data-stu-id="5fc1d-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="5fc1d-107">يمكن ان يكون سبب هذا الخطا اختناق داخل خدمه SharePoint.</span><span class="sxs-lookup"><span data-stu-id="5fc1d-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="5fc1d-108">يستخدم SharePoint علي الإنترنت اختناق للحفاظ علي الأداء الأمثل والاعتمادية لخدمه SharePoint علي الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="5fc1d-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="5fc1d-109">يحد الاختناق من عدد إجراءات المستخدم أو المكالمات المتزامنة (بواسطة البرنامج النصي أو التعليمات البرمجية) لمنع الإفراط في استخدام الموارد.</span><span class="sxs-lookup"><span data-stu-id="5fc1d-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="5fc1d-110">لمزيد من المعلومات حول اختناق راجع ، [تجنب الحصول علي مخنوق أو حظر في SharePoint علي الإنترنت](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="5fc1d-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="5fc1d-111">إذا واجهت أداء بطيء مع موقع أو صفحه SharePoint **كلاسيكية** أو **حديثه** ، استخدم [أداه تشخيص الصفحة](https://aka.ms/perftool) لتحليل الصفحات.</span><span class="sxs-lookup"><span data-stu-id="5fc1d-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="5fc1d-112">إذا كنت لا تزال تواجه أداء بطيء عام ، الرجاء مراجعه الموارد في الجزء السفلي من هذه المقالة: [مقدمه لضبط الأداء ل SharePoint علي الإنترنت](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="5fc1d-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  