---
title: مشكلات الأداء-SharePoint أو اندريف
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068373"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint أو اندريف بطيئه أو غير قابله للوصول أو غير متوفرة لعده مستخدمين

قد يكون SharePoint أو OneDrive بطيئا أو غير قابل للوصول أو غير متوفر أو قد يعرض الخدمة غير متوفرة أو أخطاء 503 لعده أسباب:
  
- إذا كان موقع SharePoint أو OneDrive الخاص بك بطيئا أو مؤجلا لعده مستخدمين ، قد تكون هناك مشكله خدمه مؤقته حيث يواجه المستخدمون تاخيرات متقطعه أو أخطاء في التنقل عند الوصول إلى مواقع SharePoint أو محتوي OneDrive. تحقق من [لوحه معلومات صحة الخدمة](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) لمعرفه ما إذا كانت مؤسستك قد تاثرت.
  
- قد يتلقى المستخدمون *ملقم 503 هو خطا مشغول* عند محاولة الانتقال إلى مواقع SharePoint أو اندريف. يمكن ان يكون سبب هذا الخطا اختناق داخل خدمه SharePoint. يستخدم SharePoint علي الإنترنت اختناق للحفاظ علي الأداء الأمثل والاعتمادية لخدمه SharePoint علي الإنترنت. يحد الاختناق من عدد إجراءات المستخدم أو المكالمات المتزامنة (بواسطة البرنامج النصي أو التعليمات البرمجية) لمنع الإفراط في استخدام الموارد. لمزيد من المعلومات حول اختناق راجع ، [تجنب الحصول علي مخنوق أو حظر في SharePoint علي الإنترنت](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- إذا واجهت أداء بطيء مع موقع أو صفحه SharePoint **كلاسيكية** أو **حديثه** ، استخدم [أداه تشخيص الصفحة](https://aka.ms/perftool) لتحليل الصفحات.
  
- إذا كنت لا تزال تواجه أداء بطيء عام ، الرجاء مراجعه الموارد في الجزء السفلي من هذه المقالة: [مقدمه لضبط الأداء ل SharePoint علي الإنترنت](https://go.microsoft.com/fwlink/?linkid=2024334)
  