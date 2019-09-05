---
title: تثبوت شيربوينت على الإنترنت
ms.author: pebaum
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: d9e1400697b1e6435fea78703d2ecadc6733a57f
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751875"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="ea7fa-102">تثبوت شيربوينت على الإنترنت</span><span class="sxs-lookup"><span data-stu-id="ea7fa-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="ea7fa-103">قد يتلقى المستخدمون ملقم 503 خطأ مشغول عند محاولة الانتقال إلى مواقع SharePoint أو أندريف.</span><span class="sxs-lookup"><span data-stu-id="ea7fa-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="ea7fa-104">يمكن أن يحدث هذا الخطأ عن طريق اختناق داخل خدمة SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ea7fa-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="ea7fa-105">يستخدم SharePoint Online اختناق للحفاظ على الأداء الأمثل والموثوقية لخدمة SharePoint عبر الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="ea7fa-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="ea7fa-106">يحدد التجلط عن عدد إجراءات المستخدم أو الاستدعاءات المتزامنة (حسب البرنامج النصي أو التعليمات البرمجية) لمنع الإفراط في استخدام الموارد.</span><span class="sxs-lookup"><span data-stu-id="ea7fa-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="ea7fa-107">إذا كنت لا تحصل على خنق، 99٪ من الوقت هو بسبب التعليمات البرمجية المخصصة.</span><span class="sxs-lookup"><span data-stu-id="ea7fa-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="ea7fa-108">لمزيد من المعلومات حول اختناق راجع، [تجنب الحصول على خنق أو حظر في SharePoint على الإنترنت](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="ea7fa-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="ea7fa-109">إذا كنت تعتقد أن هذا الخطأ لا علاقة له باختناق، يمكنك التحقق مما إذا كانت هناك صيانة نشطة تحدث على المستأجر الخاص بك عن طريق التنقل إلى [مركز الرسائل](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="ea7fa-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="ea7fa-110">وأخيراً، تأكد من زيارة صفحة ["صحة الخدمة"](https://portal.office.com/adminportal/home#/servicehealth) للتحقق من وجود أي نصائح/حوادث قد تحدث.</span><span class="sxs-lookup"><span data-stu-id="ea7fa-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

