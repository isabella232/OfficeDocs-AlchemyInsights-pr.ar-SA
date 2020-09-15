---
title: المشاركة مع المستخدمين الخارجيين لا يعملون
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
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691562"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>إصلاح المشاكل المتعلقة بمشاركه محتوي SharePoint مع مستخدمين خارجيين

تاكد من تشغيل المشاركة الخارجية لمؤسسك:
  
1. انتقل إلى [ &amp; صفحه الوظائف الاضافيه الخاصة بالخدمات في مركز أداره Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)، وانقر فوق **المواقع**.
    
2. تاكد من ان الاعداد في وضع التشغيل. إذا تم تحديد "مستخدمين خارجيين فقط" ، فتاكد من ان المستخدم الخارجي مدرج في مركز أداره Microsoft 365.
    
تاكد من تشغيل المشاركة الخارجية للموقع. بالنسبة إلى مجموعه المواقع المشتركة التقليدية:
  
1. في مركز أداره SharePoint الجديد ، في الجزء الأيمن ، انقر فوق **المواقع**.
    
2. حدد الموقع أو المواقع ، وعلي الشريط ، انقر فوق **مشاركه**.
    
بالنسبة إلى موقع الفريق الذي ينتمي إلى مجموعه Microsoft 365 أو موقع اتصال:
  
- تتضمن أنواع المواقع الجديدة هذه إعدادات المشاركة نفسها التي يستخدمها الاعداد علي مستوي المؤسسة ، ما لم يكن الاعداد علي مستوي المؤسسة يسمح بمشاركه الملفات باستخدام الارتباطات التي لا تتطلب تسجيل الدخول. في هذه الحالة ، تسمح المواقع بالمشاركة مع المستخدمين الخارجيين الجدد والموجودين الذين قاموا بتسجيل الدخول. لتغيير اعداد مواقع معينه ، استخدم مركز أداره SharePoint الجديد أو PowerShell. [تعرّف على المزيد](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> يمكن ان يكون اعداد المشاركة الخارجية لأي موقع أكثر تقييدا من الاعداد علي مستوي المؤسسة ، ولكن لا يمكنك القيام بالمزيد من الاتاحه من الاعداد علي مستوي المؤسسة. 
  

