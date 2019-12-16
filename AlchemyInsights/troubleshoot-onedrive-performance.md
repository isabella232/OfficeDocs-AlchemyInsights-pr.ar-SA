---
title: استكشاف أخطاء أداء OneDrive وإصلاحها
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 5416da63851de8b0b45e1d5c0cef24b03db40e6e
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054941"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="66ebb-102">استكشاف أخطاء أداء OneDrive وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="66ebb-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="66ebb-103">إذا كنت تواجه مزامنة إبطا من المتوقع أو مشكلات أداء مشابهه مع اندريف:</span><span class="sxs-lookup"><span data-stu-id="66ebb-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="66ebb-104">تاكد من عدم وجود مشكلات معروفه باستخدام " [لوحه معلومات صحة الخدمة](https://portal.office.com/adminportal/home?ref=/servicehealth)".</span><span class="sxs-lookup"><span data-stu-id="66ebb-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="66ebb-105">[تمكين الملفات عند الطلب](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-US&rs=en-US&ad=US) بحيث يمكنك الوصول إلى كافة الملفات الخاصة بك في OneDrive دون الحاجة إلى تحميل كل منها واستخدام مساحة التخزين علي جهازك.</span><span class="sxs-lookup"><span data-stu-id="66ebb-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-US&rs=en-US&ad=US) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="66ebb-106">[مراجعه أفضل الممارسات](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) لتخطيط الشبكة وأداءها.</span><span class="sxs-lookup"><span data-stu-id="66ebb-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="66ebb-107">[تعظيم سرعه التحميل والتنزيل](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43)، خاصه إذا كنت تقوم بمزامنة جهاز للمرة الاولي.</span><span class="sxs-lookup"><span data-stu-id="66ebb-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="66ebb-108">إذا كنت تقوم بمزامنة مكتبه بعناصر أكثر من 100,000 ، فقد تبدو مزامنة OneDrive عالقه لفتره طويلة ، أو تظهر الحالة معالجه 0KB من xMB. "</span><span class="sxs-lookup"><span data-stu-id="66ebb-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="66ebb-109">[تعرف علي مزيد من المعلومات حول مزامنة أكثر من 100,000 ملف](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) بالاضافه إلى [الحد المدعوم من ملفات 300,000 من OneDrive](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span><span class="sxs-lookup"><span data-stu-id="66ebb-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="66ebb-110">عندما يتجاوز مستخدم حدود الاستخدام ، throttles SharePoint علي الإنترنت اي طلبات أخرى من حساب المستخدم هذا لفتره قصيرة.</span><span class="sxs-lookup"><span data-stu-id="66ebb-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="66ebb-111">يتم مخنوق كافة إجراءات المستخدم اثناء الكبح في الواقع.</span><span class="sxs-lookup"><span data-stu-id="66ebb-111">All user actions are throttled while the throttle is in effect.</span></span>
