---
title: كبح SharePoint على الإنترنت
ms.author: kirks
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: c7881c0c7331e0aa74fcc439f52157bb75a56160
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559801"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="57f09-102">كبح SharePoint على الإنترنت</span><span class="sxs-lookup"><span data-stu-id="57f09-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="57f09-103">قد يتلقى المستخدمون 503 الخادم مشغول خطأ عند محاولة الانتقال إلى موقع SharePoint أو أندريف.</span><span class="sxs-lookup"><span data-stu-id="57f09-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="57f09-104">هذا الخطأ قد يتسبب بالتحكم في الخدمة SharePoint.</span><span class="sxs-lookup"><span data-stu-id="57f09-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="57f09-105">SharePoint على الإنترنت يستخدم التحكم للمحافظة على أفضل أداء وموثوقية الخدمة SharePoint على الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="57f09-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="57f09-106">التحكم بحدود عدد إجراءات المستخدم أو المتزامنة يستدعي (بواسطة برنامج نصي أو تعليمات برمجية) لمنع الإفراط في استخدام الموارد.</span><span class="sxs-lookup"><span data-stu-id="57f09-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="57f09-107">إذا كان يمكنك الحصول على التحكم، 99% الوقت وبسبب تعليمات برمجية مخصصة.</span><span class="sxs-lookup"><span data-stu-id="57f09-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="57f09-108">لمزيد من المعلومات حول التحكم، راجع [تجنب الحصول على التحكم أو حظر في SharePoint على الإنترنت](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="57f09-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="57f09-109">إذا كنت تعتقد أن هذا الخطأ غير متعلق بالتحكم، يمكنك التحقق من ما إذا كان هناك الصيانة الفعالة التي تحدث على المستأجر الخاص بك عن طريق الانتقال إلى [مركز الرسائل](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="57f09-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="57f09-110">أخيرا، تحقق من أن تقوم بزيارة صفحة [الحماية خدمة](https://portal.office.com/adminportal/home#/servicehealth) للتحقق من وجود أية نصائح/الحوادث التي قد تحدث.</span><span class="sxs-lookup"><span data-stu-id="57f09-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

