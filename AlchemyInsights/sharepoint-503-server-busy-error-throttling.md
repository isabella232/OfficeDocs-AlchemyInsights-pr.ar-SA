---
title: تقييد SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 21d0f8d0118d92562b425921742513157563b5fb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773834"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="a2706-102">تقييد SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="a2706-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="a2706-103">**هام**: خلال هذه الأوقات غير المسبوقة، نقوم باتخاذ الخطوات اللازمة لضمان توفر خدمات SharePoint Online و OneDrive بشكل كبير – الرجاء زيارة [تعديلات الميزات المؤقتة لـ SharePoint Online](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="a2706-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="a2706-104">**خادم 503 الخطا مشغول**</span><span class="sxs-lookup"><span data-stu-id="a2706-104">**503 server is busy error**</span></span>

<span data-ttu-id="a2706-105">قد يتلقى المستخدمون خطا في 503 الخادم عند محاولة الانتقال إلى مواقع SharePoint أو OneDrive.</span><span class="sxs-lookup"><span data-stu-id="a2706-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="a2706-106">قد يعود سبب هذا الخطا إلى التحكم في خدمه SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a2706-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="a2706-107">يستخدم SharePoint Online التقييد للمحافظة على الأداء الأمثل وإمكانية الاعتماد على خدمة SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="a2706-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="a2706-108">يحد التقييد من عدد إجراءات المستخدم أو المكالمات المتزامنة (بواسطة البرنامج النصي أو التعليمات البرمجية) لمنع الاستخدام المفرط للموارد.</span><span class="sxs-lookup"><span data-stu-id="a2706-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="a2706-109">للحصول علي مزيد من المعلومات حول التحكم ، يمكنك [تجنب الوصول إلى SharePoint Online أو حظره](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="a2706-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="a2706-110">إذا كنت تعتقد ان هذا الخطا غير متعلق بالتقييد ، يمكنك التحقق من وجود صيانة نشطه علي المستاجر عن طريق الانتقال إلى [مركز الرسائل](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="a2706-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="a2706-111">أخيرا ، تاكد من زيارة صفحه [حماية الخدمة](https://portal.office.com/adminportal/home#/servicehealth) للتحقق من اي نصائح/حوادث قد تحدث.</span><span class="sxs-lookup"><span data-stu-id="a2706-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

