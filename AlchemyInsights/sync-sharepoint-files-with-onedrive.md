---
title: استكشاف مشاكل "فتح باستخدام المستكشف" وإصلاحها في SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 8/7/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: 21a0c193b752342d47189dda73d171249153f7fc
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050800"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="5c735-102">استكشاف مشاكل "فتح باستخدام المستكشف" وإصلاحها في SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="5c735-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="5c735-103">يفتح الأمر "فتح بواسطة المستكشف" مثيلاً محلي لمستكشف Windows الذي يعرض بنية المجلد على الخادم الذي يستضيف موقع SharePoint.</span><span class="sxs-lookup"><span data-stu-id="5c735-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="5c735-104">سيتم إعلامك بذلك، ونوصي [بمزامنة ملفات SharePoint مع عميل المزامنة من OneDrive الجديد](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> الذي يوفر [ملفات عند الطلب](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) نظراً لأنه يوفر وصولاً محلياً إلى ملفاتك ويقدم أفضل أداء.</span><span class="sxs-lookup"><span data-stu-id="5c735-104">This being said, we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="5c735-105">إذا كنت تريد استخدام طريقة عرض "المستكشف" بدلاً من استخدام عميل المزامنة من OneDrive الجديد، فتأكد من اتباع الخطوات وأفضل الممارسات في المقالات التالية:</span><span class="sxs-lookup"><span data-stu-id="5c735-105">If you chose to use Explorer view instead of using the new OneDrive sync client, make sure you follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="5c735-106">كيفية استخدام الأمر "فتح بواسطة المستكشف" لاستكشاف الأخطاء وإصلاحها في SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="5c735-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)

- [<span data-ttu-id="5c735-107">نسخ ملفات المكتبة أو نقلها باستخدام الأمر فتح بواسطة المستكشف</span><span class="sxs-lookup"><span data-stu-id="5c735-107">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

> [!Note]  
> <span data-ttu-id="5c735-108">لا يظهر الزر **فتح بواسطة المستكشف** في تجربة المكتبة الجديدة.</span><span class="sxs-lookup"><span data-stu-id="5c735-108">The **Open with Explorer** button doesn't appear in the new library experience.</span></span> <span data-ttu-id="5c735-109">حدد القائمة المنسدلة **عرض** في الزاوية العلوية اليسرى (اسم التغييرات المنسدلة استناداً إلى طريقة العرض الحالية)، ثم حدد **عرض في مستكشف الملفات**.</span><span class="sxs-lookup"><span data-stu-id="5c735-109">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>
>
 ><span data-ttu-id="5c735-110">يستخدم "فتح بواسطة المستكشف" في SharePoint عناصر تحكم ActiveX؛ لذا فهو مدعم فقط في Internet Explorer 10 أو 11.</span><span class="sxs-lookup"><span data-stu-id="5c735-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="5c735-111">لا يعمل "فتح بواسطة المستكشف" في Windows باستخدام Microsoft Edge أو Google Chrome أو Mozilla Firefox أو علي النظام الأساسي Mac.</span><span class="sxs-lookup"><span data-stu-id="5c735-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="5c735-112">ونظراً لهذا السبب، فقد يكون خيار "طريقة عرض المستكشف" باللون الرمادي.</span><span class="sxs-lookup"><span data-stu-id="5c735-112">Due to this reason, the Explorer View option may be grayed out.</span></span>
>
> - <span data-ttu-id="5c735-113">[سبب عدم توفر أزرار شريط SharePoint أو ظهورها باللون الرمادي](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span><span class="sxs-lookup"><span data-stu-id="5c735-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  

