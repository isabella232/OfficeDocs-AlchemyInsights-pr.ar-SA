---
title: استكشاف أخطاء أداء OneDrive وإصلاحها
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 4699f6113acd70b4778f9feeaeec012ff8fdd63f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757872"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="0c1b0-102">استكشاف أخطاء أداء OneDrive وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="0c1b0-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="0c1b0-103">إذا كنت تواجه إبطا من المزامنة المتوقعة ، أو مشاكل الأداء المشابهة في OneDrive:</span><span class="sxs-lookup"><span data-stu-id="0c1b0-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="0c1b0-104">تاكد من عدم وجود اي مشاكل معروفه باستخدام [لوحه معلومات حماية الخدمة](https://portal.office.com/adminportal/home?ref=/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="0c1b0-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="0c1b0-105">يمكنك [تمكين الملفات عند الطلب](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) بحيث تتمكن من الوصول إلى كل ملفاتك في OneDrive دون الحاجة إلى تنزيل كل منها واستخدام مساحة التخزين علي جهازك.</span><span class="sxs-lookup"><span data-stu-id="0c1b0-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="0c1b0-106">[راجع أفضل الممارسات](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) لتخطيط الشبكة وأداءها.</span><span class="sxs-lookup"><span data-stu-id="0c1b0-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="0c1b0-107">قم [بزيادة سرعه التحميل والتنزيل](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43)، خاصه إذا كنت تقوم بمزامنة جهاز للمرة الاولي.</span><span class="sxs-lookup"><span data-stu-id="0c1b0-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="0c1b0-108">إذا كنت تقوم بمزامنة مكتبه تحتوي علي أكثر من 100,000 عنصر ، فقد تبدو مزامنة OneDrive عالقه لمده طويلة ، أو تعرض الحالة العملية التي تمت فيها المعالجة 0KB بالميغا بايت. "</span><span class="sxs-lookup"><span data-stu-id="0c1b0-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="0c1b0-109">[تعرف علي المزيد حول مزامنة أكثر من 100,000 ملفات](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) بالاضافه إلى [الحد المعتمد في OneDrive لملفات 300,000](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span><span class="sxs-lookup"><span data-stu-id="0c1b0-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="0c1b0-110">عندما يتجاوز المستخدم حدود الاستخدام ، قيود SharePoint Online اي طلبات اضافيه من حساب المستخدم هذا لفتره قصيرة.</span><span class="sxs-lookup"><span data-stu-id="0c1b0-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="0c1b0-111">يتم التحكم في كل إجراءات المستخدمين اثناء سريان التحكم.</span><span class="sxs-lookup"><span data-stu-id="0c1b0-111">All user actions are throttled while the throttle is in effect.</span></span>
