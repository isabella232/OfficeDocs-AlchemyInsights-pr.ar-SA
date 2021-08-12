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
ms.openlocfilehash: 53f6fd009d3dab3cd66d33d9cd248201219caa1605c7a4e7758a5a8d720f68c2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53910353"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>إصلاح المشاكل المتعلقة بمشاركة SharePoint مع مستخدمين خارجيين

تأكد من تشغيل المشاركة الخارجية لمنظمتك:
  
1. انتقل إلى صفحة الوظائف الإضافية [ &amp; للخدمات في مركز مسؤولي Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)، وانقر فوق **مواقع**.
    
2. تأكد من تشغيل الإعداد إلى "تشغيل". إذا تم تحديد "المستخدمون الخارجيون الموجودون فقط"، فتأكد من إدراج المستخدم الخارجي في مركز مسؤولي Microsoft 365.
    
تأكد من تشغيل المشاركة الخارجية للموقع. بالنسبة إلى مجموعة مواقع ويب كلاسيكية:
  
1. في مركز إدارة SharePoint الجديد، في الجزء الأيسر، انقر فوق **المواقع**.
    
2. حدد الموقع أو المواقع، وعلى الشريط، انقر فوق **مشاركة**.
    
لموقع فريق ينتمي إلى مجموعة Microsoft 365 أو موقع اتصال:
  
- وتتضمن أنواع المواقع الجديدة هذه إعداد المشاركة نفسه الذي يحتوي عليه الإعداد على مستوى المؤسسة، إلا إذا كان الإعداد على مستوى المؤسسة يسمح بمشاركة الملفات باستخدام الارتباطات التي لا تتطلب تسجيل الدخول. في هذه الحالة، تسمح المواقع بالمشاركة مع مستخدمين خارجيين جدد وموجودين الذين سجلوا الدخول. لتغيير الإعداد لمواقع معينة، استخدم SharePoint إدارة PowerShell الجديد. [تعرّف على المزيد](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> يمكن أن يكون إعداد المشاركة الخارجية لأي موقع أكثر تقييدا من الإعداد على مستوى المؤسسة، ولكنه ليس أكثر اتساما بذاته من الإعداد على مستوى المؤسسة. 
  

