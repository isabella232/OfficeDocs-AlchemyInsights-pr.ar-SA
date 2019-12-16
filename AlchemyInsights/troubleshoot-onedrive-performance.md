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
# <a name="troubleshoot-onedrive-performance"></a>استكشاف أخطاء أداء OneDrive وإصلاحها

إذا كنت تواجه مزامنة إبطا من المتوقع أو مشكلات أداء مشابهه مع اندريف:

- تاكد من عدم وجود مشكلات معروفه باستخدام " [لوحه معلومات صحة الخدمة](https://portal.office.com/adminportal/home?ref=/servicehealth)".

- [تمكين الملفات عند الطلب](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-US&rs=en-US&ad=US) بحيث يمكنك الوصول إلى كافة الملفات الخاصة بك في OneDrive دون الحاجة إلى تحميل كل منها واستخدام مساحة التخزين علي جهازك.

- [مراجعه أفضل الممارسات](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) لتخطيط الشبكة وأداءها.

- [تعظيم سرعه التحميل والتنزيل](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43)، خاصه إذا كنت تقوم بمزامنة جهاز للمرة الاولي.

- إذا كنت تقوم بمزامنة مكتبه بعناصر أكثر من 100,000 ، فقد تبدو مزامنة OneDrive عالقه لفتره طويلة ، أو تظهر الحالة معالجه 0KB من xMB. " [تعرف علي مزيد من المعلومات حول مزامنة أكثر من 100,000 ملف](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) بالاضافه إلى [الحد المدعوم من ملفات 300,000 من OneDrive](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).

- عندما يتجاوز مستخدم حدود الاستخدام ، throttles SharePoint علي الإنترنت اي طلبات أخرى من حساب المستخدم هذا لفتره قصيرة. يتم مخنوق كافة إجراءات المستخدم اثناء الكبح في الواقع.
