---
title: SharePoint اختناق عبر الإنترنت
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 50b2c29db1fd294abe6c9e60f067156109de392b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742196"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="9db7c-102">SharePoint اختناق عبر الإنترنت</span><span class="sxs-lookup"><span data-stu-id="9db7c-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="9db7c-103">**هام**: خلال هذه الأوقات غير المسبوقة، نقوم باتخاذ الخطوات اللازمة لضمان توفر خدمات SharePoint Online و OneDrive بشكل كبير – الرجاء زيارة [تعديلات الميزات المؤقتة لـ SharePoint Online](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="9db7c-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="9db7c-104">**503 خادم خطأ مشغول**</span><span class="sxs-lookup"><span data-stu-id="9db7c-104">**503 server is busy error**</span></span>

<span data-ttu-id="9db7c-105">قد يتلقى المستخدمون ملقم 503 خطأ مشغول عند محاولة الانتقال إلى مواقع SharePoint أو OneDrive.</span><span class="sxs-lookup"><span data-stu-id="9db7c-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="9db7c-106">يمكن أن يكون سبب هذا الخطأ اختناق داخل خدمة SharePoint.</span><span class="sxs-lookup"><span data-stu-id="9db7c-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="9db7c-107">يستخدم SharePoint Online التقييد للمحافظة على الأداء الأمثل وإمكانية الاعتماد على خدمة SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="9db7c-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="9db7c-108">يحد التقييد من عدد إجراءات المستخدم أو المكالمات المتزامنة (بواسطة البرنامج النصي أو التعليمات البرمجية) لمنع الاستخدام المفرط للموارد.</span><span class="sxs-lookup"><span data-stu-id="9db7c-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="9db7c-109">لمزيد من المعلومات حول الاختناق انظر، [تجنب الحصول على خنق أو حظر في SharePoint عبر الإنترنت](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="9db7c-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="9db7c-110">إذا كنت تعتقد أن هذا الخطأ لا علاقة له بالاختناق، يمكنك التحقق مما إذا كانت هناك صيانة نشطة تحدث على المستأجر الخاص بك عن طريق التنقل إلى [مركز الرسائل](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="9db7c-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="9db7c-111">أخيرًا، تأكد من زيارة صفحة ["صحة الخدمة"](https://portal.office.com/adminportal/home#/servicehealth) للتحقق من أي تحذيرات/حوادث قد تحدث.</span><span class="sxs-lookup"><span data-stu-id="9db7c-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

