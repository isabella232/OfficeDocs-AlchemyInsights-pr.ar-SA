---
title: SharePoint اختناق عبر الإنترنت
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 2aca55ac2fefbb2035140a759a77730dc905a4e9
ms.sourcegitcommit: 926e4ab6aa64ddc7a244de633421eb2b817541f2
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/26/2020
ms.locfileid: "42958705"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="b6610-102">SharePoint اختناق عبر الإنترنت</span><span class="sxs-lookup"><span data-stu-id="b6610-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="b6610-103">**هام:** خلال هذه الأوقات غير المسبوقة، نتخذ خطوات لضمان أن تظل خدمات SharePoint Online و OneDrive متاحة للغاية - يرجى زيارة [SharePoint Online تعديلات الميزة المؤقتة](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="b6610-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="b6610-104">**503 خادم خطأ مشغول**</span><span class="sxs-lookup"><span data-stu-id="b6610-104">**503 server is busy error**</span></span>

<span data-ttu-id="b6610-105">قد يتلقى المستخدمون ملقم 503 خطأ مشغول عند محاولة الانتقال إلى مواقع SharePoint أو OneDrive.</span><span class="sxs-lookup"><span data-stu-id="b6610-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="b6610-106">يمكن أن يكون سبب هذا الخطأ اختناق داخل خدمة SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b6610-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="b6610-107">يستخدم SharePoint Online الاختناق للحفاظ على الأداء الأمثل وموثوقية خدمة SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="b6610-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="b6610-108">الاختناق يحد من عدد إجراءات المستخدم أو المكالمات المتزامنة (بواسطة البرنامج النصي أو التعليمات البرمجية) لمنع الإفراط في استخدام الموارد.</span><span class="sxs-lookup"><span data-stu-id="b6610-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="b6610-109">لمزيد من المعلومات حول الاختناق انظر، [تجنب الحصول على خنق أو حظر في SharePoint عبر الإنترنت](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="b6610-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="b6610-110">إذا كنت تعتقد أن هذا الخطأ لا علاقة له بالاختناق، يمكنك التحقق مما إذا كانت هناك صيانة نشطة تحدث على المستأجر الخاص بك عن طريق التنقل إلى [مركز الرسائل](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="b6610-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="b6610-111">أخيرًا، تأكد من زيارة صفحة ["صحة الخدمة"](https://portal.office.com/adminportal/home#/servicehealth) للتحقق من أي تحذيرات/حوادث قد تحدث.</span><span class="sxs-lookup"><span data-stu-id="b6610-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

