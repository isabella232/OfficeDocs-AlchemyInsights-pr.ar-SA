---
title: استكشاف أداء OneDrive وإصلاحها
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 197a84c5f69f9e58460925049345263743fe78ee
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43733185"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="b5104-102">استكشاف أداء OneDrive وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="b5104-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="b5104-103">إذا كنت تواجه مزامنة أبطأ من المتوقع، أو مشكلات أداء مشابهة مع OneDrive:</span><span class="sxs-lookup"><span data-stu-id="b5104-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="b5104-104">تأكد من عدم وجود مشكلات معروفة باستخدام [لوحة معلومات صحة الخدمة](https://portal.office.com/adminportal/home?ref=/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="b5104-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="b5104-105">[تمكين الملفات عند الطلب](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) بحيث يمكنك الوصول إلى جميع ملفاتك في OneDrive دون الحاجة إلى تنزيلها جميعًا واستخدام مساحة التخزين على جهازك.</span><span class="sxs-lookup"><span data-stu-id="b5104-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="b5104-106">[مراجعة أفضل الممارسات](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) لتخطيط الشبكة وأدائها.</span><span class="sxs-lookup"><span data-stu-id="b5104-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="b5104-107">[قم بزيادة سرعة التحميل والتنزيل](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43)إلى أقصى حد ، خاصة إذا كنت تقوم بمزامنة جهاز لأول مرة.</span><span class="sxs-lookup"><span data-stu-id="b5104-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="b5104-108">إذا كنت تقوم بمزامنة مكتبة مع أكثر من 100,000 عنصر، فقد تبدو مزامنة OneDrive عالقة لفترة طويلة، أو تظهر الحالة معالجة 0KB من xMB."</span><span class="sxs-lookup"><span data-stu-id="b5104-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="b5104-109">[تعرف على المزيد حول مزامنة أكثر من 100,000 ملف](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) بالإضافة إلى [حد OneDrive المدعوم البالغ 300,000 ملف.](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa)</span><span class="sxs-lookup"><span data-stu-id="b5104-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="b5104-110">عندما يتجاوز المستخدم حدود الاستخدام، يخنق SharePoint Online أي طلبات أخرى من حساب المستخدم هذا لفترة قصيرة.</span><span class="sxs-lookup"><span data-stu-id="b5104-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="b5104-111">يتم خنق كافة إجراءات المستخدم أثناء سريان الخانق.</span><span class="sxs-lookup"><span data-stu-id="b5104-111">All user actions are throttled while the throttle is in effect.</span></span>
