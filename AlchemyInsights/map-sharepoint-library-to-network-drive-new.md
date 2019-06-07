---
title: تعيين مكتبة SharePoint إلى محرك أقراص شبكة الاتصال
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 12/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 4b8245c3-a179-4524-ae83-0c22d539c202
ms.openlocfilehash: 7bb1f7d1b77ec5850109c9553ddfd894b3823946
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/07/2019
ms.locfileid: "34754802"
---
# <a name="map-a-sharepoint-library-to-a-network-drive"></a><span data-ttu-id="cda0f-102">تعيين مكتبة SharePoint إلى محرك أقراص شبكة الاتصال</span><span class="sxs-lookup"><span data-stu-id="cda0f-102">Map a SharePoint library to a network drive</span></span>

<span data-ttu-id="cda0f-103">يتم تعيين مكتبة كمحرك أقراص شبكة المؤقتة والمعتمدة فقط من خلال Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="cda0f-103">Mapping a library as a network drive is temporary and supported only through Internet Explorer.</span></span> <span data-ttu-id="cda0f-104">أحياناً يجب فتح موقع SharePoint في برنامج Internet Explorer وحدد "الاحتفاظ بتسجيل الدخول" لمنع انتهاء مدة صلاحية جلسة العمل.</span><span class="sxs-lookup"><span data-stu-id="cda0f-104">You must occasionally open the SharePoint site in Internet Explorer and select "Stay signed in" to prevent the session from expiring.</span></span> <span data-ttu-id="cda0f-105">بدلاً من ذلك، [مزامنة الملفات SharePoint باستخدام عميل المزامنة الجديدة أندريف](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88) </a> التي توفر [الملفات عند الطلب](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e).</span><span class="sxs-lookup"><span data-stu-id="cda0f-105">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e).</span></span> <span data-ttu-id="cda0f-106">الوصول إلى كافة الملفات في أندريف دون استخدام مساحة للتخزين المحلي.</span><span class="sxs-lookup"><span data-stu-id="cda0f-106">Access all your files in OneDrive without using local storage space.</span></span>

<span data-ttu-id="cda0f-107">إذا اخترت تعيين محرك أقراص بدلاً من[استخدام عميل المزامنة أونيدريفي الجديد](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)، تأكد من اتباع الخطوات الواردة في المقالة أدناه.</span><span class="sxs-lookup"><span data-stu-id="cda0f-107">If you choose to map a drive instead of[using the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88), ensure you follow the steps in the article below.</span></span> 


<span data-ttu-id="cda0f-108">**محركات أقراص الشبكة المعينة كيفية تكوين واستكشاف الأخطاء وإصلاحها**</span><span class="sxs-lookup"><span data-stu-id="cda0f-108">**How to configure and troubleshoot mapped network drives**</span></span>


- <span data-ttu-id="cda0f-109">[تكوين ومحركات أقراص الشبكة المعينة لاستكشاف الأخطاء وإصلاحها](https://support.office.com/article/troubleshoot-mapped-network-drives-that-connect-to-sharepoint-online-ef399c67-4578-4c3a-adbe-0b489084eabe?ui=en-US&amp;rs=en-US&amp;ad=US).</span><span class="sxs-lookup"><span data-stu-id="cda0f-109">[Configure and to troubleshoot mapped network drives](https://support.office.com/article/troubleshoot-mapped-network-drives-that-connect-to-sharepoint-online-ef399c67-4578-4c3a-adbe-0b489084eabe?ui=en-US&amp;rs=en-US&amp;ad=US).</span></span>

<span data-ttu-id="cda0f-110">ملاحظة: لبرنامج Internet Explorer 10 مع ويندوز 8 أو ويندوز 7 تلقي "رفض الوصول" أو "مسار غير قابل للوصول" عند تعيين محرك أقراص، تثبيت هذا الإصلاح العاجل لحل هذه المشكلة.</span><span class="sxs-lookup"><span data-stu-id="cda0f-110">NOTE:  For Internet Explorer 10 with Windows 8 or Windows 7 that receive "Access denied" or "Path is not accessible" when mapping a drive, install this hotfix to resolve this problem.</span></span> <span data-ttu-id="cda0f-111">الانتقال إلى [الخطأ عندما تقوم بفتح مكتبة مستندات SharePoint في "مستكشف Windows" أو تعيين محرك أقراص شبكة اتصال لمكتبة بعد تثبيت Internet Explorer 10](https://support.microsoft.com/help/2846960).</span><span class="sxs-lookup"><span data-stu-id="cda0f-111">Go to [Error when you open a SharePoint Document Library in Windows Explorer or map a network drive to the library after you install Internet Explorer 10](https://support.microsoft.com/help/2846960).</span></span>
