---
title: مشاكل الأداء SharePoint أو OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 921aae7eba8487c5600f290fd671ef2675372e6af0478b913e38354856cbaa22
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911829"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint أو OneDrive بطيئة أو يتعذر الوصول إليها أو غير متوفرة لعدة مستخدمين

SharePoint أو OneDrive يكون بطيئا أو يتعذر الوصول إليه أو غير متوفر، أو قد يعرض الخدمة غير متوفرة أو 503 أخطاء، لعدة أسباب:
  
- إذا كان SharePoint أو OneDrive الخاص بك بطيئا أو متأخرا لعدة مستخدمين، فقد تكون هناك مشكلة خدمة مؤقتة حيث تواجه المستخدمون تأخيرات متقطعة أو أخطاء في التنقل عند الوصول إلى مواقع SharePoint أو OneDrive المحتويات. تحقق من [لوحة معلومات حالة الخدمة](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) لمعرفة ما إذا كانت مؤسستك متأثّر بها.
  
- قد يتلقى المستخدمون خطأ مشغولا في *خادم 503* عند محاولة الانتقال إلى SharePoint أو OneDrive ويب. يمكن أن يحدث هذا الخطأ عن طريق التكبل داخل SharePoint الخدمة. يستخدم SharePoint Online التقييد للمحافظة على الأداء الأمثل وإمكانية الاعتماد على خدمة SharePoint Online. يحد التقييد من عدد إجراءات المستخدم أو المكالمات المتزامنة (بواسطة البرنامج النصي أو التعليمات البرمجية) لمنع الاستخدام المفرط للموارد. للحصول على مزيد من المعلومات حول الكبح، راجع تجنب التعرض [لحظر](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)أو الغلق في SharePoint Online .

- إذا واجهت أداء بطيئا **باستخدام** موقع أو صفحة SharePoint كلاسيكي [](https://aka.ms/perftool) أو حديث، فاستعين بأداة تشخيص الصفحة لتحليل الصفحات. 
  
- إذا ما زلت تواجه أداء بطيئا عاما، فالرجاء مراجعة الموارد في أسفل هذه المقالة: مقدمة حول ضبط الأداء [ل SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  