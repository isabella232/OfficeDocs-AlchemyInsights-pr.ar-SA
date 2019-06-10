---
title: مزامنة ملفات SharePoint باستخدام عميل المزامنة من OneDrive الجديد
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 5/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: 74b79efeb7e46d03dc55f46252d152cd13e66c84
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757783"
---
# <a name="sync-sharepoint-files-with-the-new-onedrive-sync-client"></a><span data-ttu-id="4db02-102">مزامنة ملفات SharePoint باستخدام عميل المزامنة من OneDrive الجديد</span><span class="sxs-lookup"><span data-stu-id="4db02-102">Sync SharePoint files with the new OneDrive sync client</span></span>

<span data-ttu-id="4db02-103">يفتح الأمر "فتح بواسطة المستكشف" مثيلاً محلي لمستكشف Windows الذي يعرض بنية المجلد على الخادم الذي يستضيف موقع SharePoint.</span><span class="sxs-lookup"><span data-stu-id="4db02-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="4db02-104">ونوصي [بمزامنة ملفات SharePoint مع عميل المزامنة من OneDrive الجديد](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> الذي يوفر [ملفات عند الطلب](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) نظراً لأنه يوفر وصولاً محلياً إلى ملفاتك ويقدم أفضل أداء.</span><span class="sxs-lookup"><span data-stu-id="4db02-104">This being said , we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="4db02-105">إذا كنت تريد استخدام طريقة عرض "المستكشف" بدلاً من استخدام عميل المزامنة الجديد، فتأكد من اتباع الخطوات وأفضل الممارسات في المقالات الموجودة أدناه.</span><span class="sxs-lookup"><span data-stu-id="4db02-105">If you chose to use explorer view instead of using the new sync client, ensure you follow the steps and best practices in the articles below.</span></span>

- [<span data-ttu-id="4db02-106">كيفية استخدام الأمر "فتح بواسطة المستكشف" لاستكشاف الأخطاء وإصلاحها في SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="4db02-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)

- [<span data-ttu-id="4db02-107">نسخ ملفات المكتبة أو نقلها باستخدام الأمر فتح بواسطة المستكشف</span><span class="sxs-lookup"><span data-stu-id="4db02-107">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

<span data-ttu-id="4db02-108">ملاحظه: لا يظهر الزر "فتح بواسطة المستكشف" في تجربة المكتبة الجديدة.</span><span class="sxs-lookup"><span data-stu-id="4db02-108">Note:  The Open with Explorer button doesn't appear in the new library experience.</span></span> <span data-ttu-id="4db02-109">انقر فوق القائمة المنسدلة "عرض" في الزاوية العلوية اليسرى (اسم التغييرات المنسدلة استناداً إلى طريقة العرض الحالية)، ثم انقر فوق "عرض في مستكشف الملفات".</span><span class="sxs-lookup"><span data-stu-id="4db02-109">Click the View drop-down in the upper right (the name of the drop-down changes depending on your current view), and then click View in File Explorer.</span></span>

 <span data-ttu-id="4db02-110">يستخدم "فتح بواسطة المستكشف" في SharePoint عناصر تحكم ActiveX؛ لذا فهو مدعم فقط في Internet Explorer 10 أو 11.</span><span class="sxs-lookup"><span data-stu-id="4db02-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="4db02-111">لا يعمل "فتح بواسطة المستكشف" في Windows باستخدام Microsoft Edge أو Google Chrome أو Mozilla Firefox أو علي النظام الأساسي Mac.</span><span class="sxs-lookup"><span data-stu-id="4db02-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="4db02-112">ونظراً لهذا السبب، فقد يكون خيار "طريقة عرض المستكشف" باللون الرمادي.</span><span class="sxs-lookup"><span data-stu-id="4db02-112">Due to this reason, the Explorer View option may be grayed out.</span></span>

- <span data-ttu-id="4db02-113">[سبب عدم توفر أزرار شريط SharePoint أو ظهورها باللون الرمادي](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span><span class="sxs-lookup"><span data-stu-id="4db02-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  

