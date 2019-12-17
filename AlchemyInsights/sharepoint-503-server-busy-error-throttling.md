---
title: اختناق SharePoint علي الإنترنت
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: ed3598dc92a7c36c9c9b077db0ab31f63537ef60
ms.sourcegitcommit: 14894a09db1c4101e48ff720d878d1c9f7b1dac8
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/16/2019
ms.locfileid: "40065545"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="1de2f-102">اختناق SharePoint علي الإنترنت</span><span class="sxs-lookup"><span data-stu-id="1de2f-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="1de2f-103">قد يتلقى المستخدمون ملقم 503 خطا مشغول عند محاولة الانتقال إلى مواقع SharePoint أو اندريف.</span><span class="sxs-lookup"><span data-stu-id="1de2f-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="1de2f-104">يمكن ان يكون سبب هذا الخطا اختناق داخل خدمه SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1de2f-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="1de2f-105">يستخدم SharePoint علي الإنترنت اختناق للحفاظ علي الأداء الأمثل والاعتمادية لخدمه SharePoint علي الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="1de2f-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="1de2f-106">يحد الاختناق من عدد إجراءات المستخدم أو المكالمات المتزامنة (بواسطة البرنامج النصي أو التعليمات البرمجية) لمنع الإفراط في استخدام الموارد.</span><span class="sxs-lookup"><span data-stu-id="1de2f-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="1de2f-107">لمزيد من المعلومات حول اختناق راجع ، [تجنب الحصول علي مخنوق أو حظر في SharePoint علي الإنترنت](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="1de2f-107">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="1de2f-108">إذا كنت تعتقد ان هذا الخطا لا علاقة له بالاختناق ، يمكنك التحقق مما إذا كان هناك صيانة نشطه تحدث علي المستاجر الخاص بك عن طريق الانتقال إلى [مركز الرسائل](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="1de2f-108">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="1de2f-109">وأخيرا ، تاكد من زيارة صفحه [الخدمة الصحية](https://portal.office.com/adminportal/home#/servicehealth) للتحقق من وجود اي تحذيرات/حوادث قد تحدث.</span><span class="sxs-lookup"><span data-stu-id="1de2f-109">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

