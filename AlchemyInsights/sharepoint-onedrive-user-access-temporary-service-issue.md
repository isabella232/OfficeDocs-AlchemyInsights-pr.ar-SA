---
title: مشاكل الأداء-SharePoint أو OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771231"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint أو OneDrive البطيء أو القابل للوصول أو غير المتاح لعده مستخدمين

إذا لم يكن موقع OneDrive أو SharePoint متوفرا لعده مستخدمين لديهم حق الوصول ، فقد تكون هناك مشكله خدمه مؤقته. [تحقق من لوحه معلومات حماية الخدمة](https://portal.office.com/adminportal/home#/servicehealth).

**أضافه المستخدم وترخيصه**

تاكد من [تعيين تراخيص للمستخدمين في Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).


**تعيين الأذونات**

إذا تم تعيين ترخيص Sharepoint إلى المستخدم وكان لا يزال يتلقى رسالة برفض الوصول ، فالرجاء التاكد من انه تم تعيين [مستوي الأذونات المناسب](https://docs.microsoft.com/sharepoint/understanding-permission-levels) لها.

**خذ في الاعتبار استخدام ميزه طلبات الوصول**

تسمح [ميزه طلبات access](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) للأشخاص بطلب الوصول إلى المحتوي الذي لا يملكون الاذن بالاطلاع عليه حاليا.

**قد يؤدي السماح بالبرنامج النصي المخصص إلى مشاكل رفض الوصول**

هناك بعض السيناريوهات التي قد يكون فيها *السماح لميزه البرامج النصية المخصصة* بتقديم رفض الوصول. للحصول علي قائمه بالميزات المتاثره ، واعتبارات الأمان والقدرة علي تعطيل الميزة. يرجى زيارة [السماح بالبرامج النصية المخصصة أو منعها](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

