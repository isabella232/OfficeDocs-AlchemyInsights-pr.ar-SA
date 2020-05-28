---
title: استكشاف مشاكل "فتح باستخدام المستكشف" وإصلاحها في SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: be1136f7fd4575d482d38ee70163e5252d4ffbca
ms.sourcegitcommit: 5296874062b16f945d9a7a7a9ab29ec53686310b
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/21/2020
ms.locfileid: "44343168"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="7297b-102">استكشاف مشاكل "فتح باستخدام المستكشف" وإصلاحها في SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="7297b-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="7297b-103">نوصي [بمزامنة ملفات SharePoint مع عميل المزامنة من OneDrive الجديد](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88) الذي يوفر [ملفات عند الطلب](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) نظراً لأنه يوفر وصولاً محلياً إلى ملفاتك ويقدم أفضل أداء.</span><span class="sxs-lookup"><span data-stu-id="7297b-103">We recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88) which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>

<span data-ttu-id="7297b-104">لاستكشاف مشاكل "فتح بواسطة مستكشف"، اتبع الخطوات وأفضل الممارسات في المقالات التالية:</span><span class="sxs-lookup"><span data-stu-id="7297b-104">To troubleshoot Open with Explorer issues, follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="7297b-105">كيفية استخدام الأمر "فتح بواسطة المستكشف" لاستكشاف الأخطاء وإصلاحها في SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="7297b-105">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)
- [<span data-ttu-id="7297b-106">نسخ ملفات المكتبة أو نقلها باستخدام الأمر فتح بواسطة المستكشف</span><span class="sxs-lookup"><span data-stu-id="7297b-106">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

> <span data-ttu-id="7297b-107">**ملاحظة:**</span><span class="sxs-lookup"><span data-stu-id="7297b-107">**Note:**</span></span>
>- <span data-ttu-id="7297b-108">"فتح بواسطة المستكشف" معتمد فقط في Internet Explorer 10 أو 11.</span><span class="sxs-lookup"><span data-stu-id="7297b-108">Open with Explorer is only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="7297b-109">لا يعمل "فتح بواسطة المستكشف" في Windows باستخدام Microsoft Edge أو Google Chrome أو Mozilla Firefox أو علي النظام الأساسي Mac.</span><span class="sxs-lookup"><span data-stu-id="7297b-109">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="7297b-110">ونظراً لهذا السبب، فقد يكون خيار "طريقة عرض المستكشف" باللون الرمادي.</span><span class="sxs-lookup"><span data-stu-id="7297b-110">Due to this reason, the Explorer View option may be grayed out.</span></span>
>
>- <span data-ttu-id="7297b-111">لا يظهر الزر "فتح بواسطة المستكشف" في تجربة المكتبة الجديدة.</span><span class="sxs-lookup"><span data-stu-id="7297b-111">The Open with Explorer button doesn't appear in the new library experience.</span></span> <span data-ttu-id="7297b-112">حدد القائمة المنسدلة **عرض** في الزاوية العلوية اليسرى (اسم التغييرات المنسدلة استناداً إلى طريقة العرض الحالية)، ثم حدد **عرض في مستكشف الملفات**.</span><span class="sxs-lookup"><span data-stu-id="7297b-112">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>
