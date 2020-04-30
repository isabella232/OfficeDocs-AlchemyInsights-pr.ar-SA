---
title: MC210173 - إهمال ميزة النموذج المخصص الجديدة في SharePoint Designer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: 185e8fc94345b240667490b1ffc63af8459d8daf
ms.sourcegitcommit: a9e6b2fcce8bd12fd079ed967f426b67d5c6d239
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/28/2020
ms.locfileid: "43928515"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a><span data-ttu-id="1296d-102">MC210173 - إهمال ميزة النموذج المخصص الجديدة في SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="1296d-102">MC210173 - SharePoint Designer new custom Form feature deprecation</span></span>

<span data-ttu-id="1296d-103">لقد عرفنا مشكلة تؤثر على وظيفة SharePoint Designer من أجل [إنشاء نماذج مخصصة](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) في SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="1296d-103">We’ve identified an issue affecting SharePoint Designer functionality for [creating custom Forms](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) within SharePoint Online.</span></span> <span data-ttu-id="1296d-104">بعد الفحص الدقيق، قررنا أنه لا يوجد حل معروف لهذه المشكلة واخترنا تعطيل ميزة إنشاء النموذج المخصصة اعتباراً من الساعة 3:00 صباحاً بالتوقيت العالمي المنسق يوم السبت 25 أبريل 2020.</span><span class="sxs-lookup"><span data-stu-id="1296d-104">After careful examination, we’ve determined that there is no known fix for this issue and have elected to disable the custom Form creation feature effective as of 3:00 AM UTC on Saturday, April 25, 2020.</span></span> <span data-ttu-id="1296d-105">لا يؤثر هذا التغيير على إمكانية تحرير النماذج التي تم إنشاؤها مسبقاً أو الميزات الموجودة الأخرى في SharePoint Online Designer.</span><span class="sxs-lookup"><span data-stu-id="1296d-105">This change does not impact the ability to edit previously created Forms or other existing features in SharePoint Online Designer.</span></span>

<span data-ttu-id="1296d-106">بعد إجراء هذا التغيير، ربما يكون المستخدمون قد تلقوا الخطأ: "تعذر حفظ تغييرات القائمة على الخادم"، عند إنشاء نماذج جديدة.</span><span class="sxs-lookup"><span data-stu-id="1296d-106">After this change was made, users may have received the error: "Could not save the list changes to the server," when creating new Forms.</span></span>

<span data-ttu-id="1296d-107">وبدلاً من ذلك، يمكن للمستخدمين الذين استفادوا من SharePoint Designer لإنشاء نماذج مخصصة استخدام [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) لهذا الغرض.</span><span class="sxs-lookup"><span data-stu-id="1296d-107">Users who have previously leveraged SharePoint Designer to create custom Forms are instead able to utilize [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) for this purpose.</span></span>

<span data-ttu-id="1296d-108">PowerApps هي أداة سهلة وفعالة تتيح للمستخدمين الذين يعملون في تجربة SharePoint Online Modern إنشاء نماذج مخصصة وتحريرها لقوائم SharePoint ومكتبات المستندات مباشرة من نافذة المستعرض.</span><span class="sxs-lookup"><span data-stu-id="1296d-108">PowerApps is an easy and powerful tool that allows users operating in the SharePoint Online Modern experience to create and edit custom Forms for SharePoint lists and document libraries right from a browser window.</span></span> <span data-ttu-id="1296d-109">لا يتطلب PowerApps معرفة التعليمات البرمجية التقليدية أو أي تنزيلات إضافية للتطبيقات مثل InfoPath.</span><span class="sxs-lookup"><span data-stu-id="1296d-109">PowerApps does not require traditional coding knowledge or any additional app downloads such as InfoPath.</span></span>

<span data-ttu-id="1296d-110">**ملاحظة**: سيحتاج مستخدمو SharePoint Online Classic إلى التبديل مؤقتاً إلى التجربة الحديثة للوصول إلى PowerApps والاستفادة منها؛ على الرغم من ذلك، يمكن الوصول إلى جميع النماذج المخصصة التي تم إنشاؤها في PowerApps بواسطة مستخدمي تجربة SharePoint Online Classic.</span><span class="sxs-lookup"><span data-stu-id="1296d-110">**Note**: SharePoint Online Classic users will need to temporarily switch to the Modern experience to access and utilize PowerApps; though, all custom Forms created in PowerApps are accessible by SharePoint Online Classic experience users.</span></span>
