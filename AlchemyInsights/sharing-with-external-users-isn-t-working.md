---
title: لا تعمل المشاركة مع مستخدمين خارجيين
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 02d79c1b1e112eb41e8c60ffa2ef28e429f76ada
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58304356"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>إصلاح المشاكل المتعلقة SharePoint المحتوى مع مستخدمين خارجيين

تأكد من تشغيل المشاركة الخارجية لمنظمتك:
  
1. انتقل إلى [صفحة الوظائف الإضافية للخدمات &amp; في](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)مركز مسؤولي Microsoft 365 ، وانقر فوق **مواقع**.
    
2. تأكد من تشغيل الإعداد إلى "تشغيل". إذا تم تحديد "المستخدمون الخارجيون الموجودون فقط"، فتأكد من إدراج المستخدم الخارجي في مركز مسؤولي Microsoft 365.
    
تأكد من تشغيل المشاركة الخارجية للموقع. بالنسبة إلى مجموعة مواقع ويب كلاسيكية:
  
1. في مركز إدارة SharePoint الجديد، في الجزء الأيسر، انقر فوق **المواقع**.
    
2. حدد الموقع أو المواقع، وعلى الشريط، انقر فوق **مشاركة**.
    
بالنسبة إلى موقع فريق ينتمي إلى مجموعة Microsoft 365 أو موقع اتصالات:
  
- تملك أنواع المواقع الجديدة هذه إعداد المشاركة نفسه الذي يحتوي عليه الإعداد على مستوى المؤسسة، إلا إذا كان الإعداد على مستوى المؤسسة يسمح بمشاركة الملفات باستخدام الارتباطات التي لا تتطلب تسجيل الدخول. في هذه الحالة، تسمح المواقع بالمشاركة مع مستخدمين خارجيين جدد وموجودين الذين سجلوا الدخول. لتغيير الإعداد لمواقع معينة، استخدم SharePoint الجديد أو PowerShell. [تعرّف على المزيد](https://go.microsoft.com/fwlink/?linkid=871863).
    
**ملاحظة:** يمكن أن يكون إعداد المشاركة الخارجية لأي موقع أكثر تقييدا من الإعداد على مستوى المؤسسة، ولكنه لا يكون أكثر اتساما بذاته من الإعداد على مستوى المؤسسة. 
  

