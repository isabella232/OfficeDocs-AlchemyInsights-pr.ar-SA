---
title: مشاكل الأداء SharePoint أو أندريف
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 3b04e811b69a1f9d652abbd603c3c09df068480c
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719504"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint أو أندريف بطيئة، غير قابلة للوصول أو غير متاحة للعديد من المستخدمين

في حالة عدم توفر للعديد من المستخدمين الذين تم الوصول إلى موقع SharePoint أو أندريف، قد يكون هناك مشكلة في خدمة مؤقت. [تحقق من لوحة المعلومات الصحية الخدمة](https://portal.office.com/adminportal/home#/servicehealth).

## <a name="add-and-license-the-user"></a>إضافة وترخيص المستخدم

تأكد من ذلك يمكنك [تعيين التراخيص للمستخدمين في Office 365 للعمل](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).


## <a name="assign-permissions"></a>تعيين أذونات

إذا تم تعيين ترخيص Sharepoint المستخدم ويزال يتلقى رسالة رفض وصول، الرجاء التأكد من لديهم [مستوى الأذونات المناسبة](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) المعينة.

## <a name="consider-using-the-access-request-feature"></a>يمكنك استخدام ميزة طلب الوصول

تسمح [ميزة طلب الوصول](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) الأشخاص لطلب الوصول إلى محتوى ليس حاليا لديهم إذن بعرضها.

## <a name="allow-custom-script-may-cause-access-denied-issues"></a>السماح بالبرامج النصية المخصصة قد يسبب مشاكل تم رفض الوصول

هناك بعض السيناريوهات حيث ميزة *السماح بالبرنامج النصي المخصص* قد يكون تقديم رفض وصول. لقائمة الميزات المتأثرة واعتبارات الأمان وإمكانية تعطيل الميزة. الرجاء زيارة [السماح أو منع البرامج النصية المخصصة](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).

