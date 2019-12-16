---
title: مشكلات الأداء-SharePoint أو اندريف
ms.author: pebaum
author: pebaum
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 2db0a9442b9fdf1752b654f7c188e641e0a274cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053788"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint أو اندريف بطيئه أو غير قابله للوصول أو غير متوفرة لمستخدمين متعددين

إذا كان موقع اندريف أو SharePoint غير متوفر للعديد من المستخدمين الذين كان لديهم حق الوصول مسبقا ، قد تكون هناك مشكله خدمه مؤقته. [تحقق من لوحه معلومات صحة الخدمة](https://portal.office.com/adminportal/home#/servicehealth).

**أضافه المستخدم وترخيصه**

تاكد من [تعيين التراخيص للمستخدمين في Office 365 للعمل](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).


**تعيين الأذونات**

إذا تم تعيين ترخيص Sharepoint للمستخدم ولا يزال يتلقى رسالة تم رفض الوصول اليها ، الرجاء التاكد من ان لديهم [مستوي الاذن المناسب](https://docs.microsoft.com/sharepoint/understanding-permission-levels) المعين.

**النظر في استخدام ميزه طلب الوصول**

تسمح [ميزه طلب الوصول](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) للأشخاص بطلب الوصول إلى المحتوي الذي ليس لديهم حاليا اذن لرؤيته.

**السماح لبرنامج نصي مخصص قد يؤدي إلى رفض الوصول المشكلات**

هناك بعض وحدات السيناريو حيث *السماح ميزه البرنامج النصي المخصص* قد يتم تقديم رفض وصول. للحصول علي قائمه بالميزات المتاثره ، اعتبارات الأمان والقدرة علي تعطيل الميزة. يرجى زيارة [السماح أو منع البرنامج النصي المخصص](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

