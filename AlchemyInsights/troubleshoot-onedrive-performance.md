---
title: استكشاف أخطاء أداء أندريف وإصلاحها
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 222f818c3fd78a19b9952d4703755498bc080910
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822185"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="57150-102">استكشاف أخطاء أداء أندريف وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="57150-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="57150-103">إذا كنت تواجه مزامنة أبطأ من المتوقع، أو مشكلات أداء مشابهة مع OneDrive:</span><span class="sxs-lookup"><span data-stu-id="57150-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="57150-104">تأكد من عدم وجود مشكلات معروفة باستخدام [لوحة معلومات صحة الخدمة](https://portal.office.com/adminportal/home?ref=/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="57150-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="57150-105">[تمكين الملفات عند الطلب](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-US&rs=en-US&ad=US) بحيث يمكنك الوصول إلى جميع الملفات الخاصة بك في OneDrive دون الحاجة إلى تحميل كل منهم واستخدام مساحة التخزين على جهازك.</span><span class="sxs-lookup"><span data-stu-id="57150-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-US&rs=en-US&ad=US) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="57150-106">[مراجعة أفضل الممارسات](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) لتخطيط الشبكة وأدائها.</span><span class="sxs-lookup"><span data-stu-id="57150-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="57150-107">[يمكنك زيادة سرعة التحميل والتنزيل إلى أقصى حد،](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43)خاصة إذا كنت تقوم بمزامنة جهاز للمرة الأولى.</span><span class="sxs-lookup"><span data-stu-id="57150-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="57150-108">إذا كنت تقوم بمزامنة مكتبة تحتوي على أكثر من 100,000 عنصر، فقد تبدو مزامنة OneDrive عالقة لفترة طويلة، أو تظهر الحالة معالجة 0 كيلو بايت من xMB."</span><span class="sxs-lookup"><span data-stu-id="57150-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="57150-109">[تعرّف على مزيد من المعلومات حول مزامنة أكثر من 100,000 ملف](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) بالإضافة إلى [الحد المعتمد من OneDrive والمحدد 300,000 ملف](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span><span class="sxs-lookup"><span data-stu-id="57150-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="57150-110">عندما يتجاوز مستخدم حدود الاستخدام، يقوم SharePoint Online بخنق أية طلبات أخرى من حساب المستخدم هذا لفترة قصيرة.</span><span class="sxs-lookup"><span data-stu-id="57150-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="57150-111">يتم خنق كافة إجراءات المستخدم أثناء خنق ساري المفعول.</span><span class="sxs-lookup"><span data-stu-id="57150-111">All user actions are throttled while the throttle is in effect.</span></span>
