---
title: استكشاف أخطاء الوصول إلى الرسائل التي تم رفضها
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: f49cfc50142b3d98a5f431a38e9a943eb5624523
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691670"
---
# <a name="troubleshoot-access-denied-messages"></a>استكشاف أخطاء الوصول إلى الرسائل التي تم رفضها

إذا تلقيت رسالة تفيد بأنه تم رفض الوصول عند محاولة استعراض موقع Sharepoint Online ، فالرجاء مراجعه المقالات التالية.

**أضافه المستخدم وترخيصه**

تاكد من [تعيين تراخيص للمستخدمين في Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).

**تعيين الأذونات**

إذا تم تعيين ترخيص Sharepoint إلى المستخدم وكان لا يزال يتلقى رسالة برفض الوصول ، فالرجاء التاكد من انه تم [تعيين مستوي الأذونات المناسب](https://docs.microsoft.com/sharepoint/understanding-permission-levels)لها.

**خذ في الاعتبار استخدام ميزه طلبات الوصول**

تسمح ميزه [طلبات access](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) للأشخاص بطلب الوصول إلى المحتوي الذي لا يملكون الاذن بالاطلاع عليه حاليا. 

**قد يؤدي السماح بالبرنامج النصي المخصص إلى مشاكل رفض الوصول**

هناك بعض السيناريوهات التي قد يكون فيها الميزة "السماح ببرمجه نصيه مخصصه" من تقديم رفض الوصول. للحصول علي قائمه بالميزات المتاثره ، واعتبارات الأمان والقدرة علي تعطيل الميزة. يرجى زيارة [برنامج نصي مخصص أو السماح به أو منعه](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

ملاحظه: إذا لم يكن موقع OneDrive أو SharePoint متوفرا لعده مستخدمين لديهم حق الوصول ، فقد تكون هناك مشكله خدمه مؤقته. [تحقق من لوحه معلومات حماية الخدمة](https://portal.office.com/adminportal/home#/servicehealth).


  

