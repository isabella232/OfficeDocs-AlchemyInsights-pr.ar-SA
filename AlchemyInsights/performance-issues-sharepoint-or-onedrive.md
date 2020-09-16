---
title: مشاكل الأداء-SharePoint أو OneDrive
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
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771888"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint أو OneDrive البطيء أو القابل للوصول أو غير متوفر لعده مستخدمين

قد يكون SharePoint أو OneDrive بطيئا أو لا يمكن الوصول اليه أو غير متاح ، أو قد يعرض الخدمة غير متوفرة أو أخطاء 503 ، لأسباب عديده:
  
- إذا كان موقع SharePoint أو OneDrive بطيئا أو متاخرا لعده مستخدمين ، فقد يكون هناك مشكله خدمه مؤقته حيث يواجه المستخدمون تاخيرات متقطعه أو أخطاء في التنقل عند الوصول إلى مواقع SharePoint أو محتوي OneDrive. راجع [لوحه معلومات حماية الخدمة](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) لمعرفه ما إذا كانت مؤسستك متاثره بالأمر.
  
- قد يتلقى المستخدمون خطا في *503 الخادم* عند محاولة الانتقال إلى مواقع SharePoint أو OneDrive. قد يعود سبب هذا الخطا إلى التحكم في خدمه SharePoint. يستخدم SharePoint Online التقييد للمحافظة على الأداء الأمثل وإمكانية الاعتماد على خدمة SharePoint Online. يحد التقييد من عدد إجراءات المستخدم أو المكالمات المتزامنة (بواسطة البرنامج النصي أو التعليمات البرمجية) لمنع الاستخدام المفرط للموارد. للحصول علي مزيد من المعلومات حول التحكم ، يمكنك [تجنب الوصول إلى SharePoint Online أو حظره](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- إذا كنت تواجه بطء في الأداء باستخدام موقع أو صفحه SharePoint **التقليدية** أو **الحديثة** ، فيمكنك استخدام [أداه تشخيص الصفحة](https://aka.ms/perftool) لتحليل الصفحات.
  
- إذا كنت لا تزال تواجه الأداء البطيء بشكل عام ، فالرجاء مراجعه الموارد في أسفل هذه المقالة: [مقدمه حول توليف الأداء ل SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  