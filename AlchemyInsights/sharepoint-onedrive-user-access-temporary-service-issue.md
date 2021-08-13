---
title: مشاكل الأداء SharePoint أو OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 08bdc2527147279063e3f66a1767203e5ccdc1dd4fd8b871f2800d3f71b9a233
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093663"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint أو OneDrive بطيئة أو غير قابلة للوصول أو غير متوفرة لمستخدمين متعددين

إذا لم OneDrive موقع ويب SharePoint لمستخدمين متعددين سبق لهم الوصول إليه، فقد تكون هناك مشكلة مؤقتة في الخدمة. [تحقق من لوحة معلومات "صحة الخدمة".](https://portal.office.com/adminportal/home#/servicehealth)

**إضافة المستخدم وترخيصه**

تأكد من تعيين التراخيص للمستخدمين في [Microsoft 365 للأعمال.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)


**تعيين الأذونات**

إذا تم تعيين ترخيص Sharepoint للمستخدم ولا يزال يتلقى رسالة رفض الوصول، فالرجاء التأكد من تعيين [مستوى](https://docs.microsoft.com/sharepoint/understanding-permission-levels) الأذونات المناسب له.

**التفكير في استخدام ميزة طلب الوصول**

تسمح [ميزة طلب الوصول](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) للأشخاص بطلب الوصول إلى المحتوى الذي ليس لديهم الإذن حاليا لمشاهدته.

**قد يتسبب السماح بالنص النصي المخصص في حدوث مشاكل في رفض الوصول**

هناك بعض السيناريوهات حيث قد تكون ميزة *السماح* بالنص النصي المخصص تعرض رفض الوصول. للحصول على قائمة بالميزات المتأثرة، اعتبارات الأمان والقدرة على تعطيل الميزة. يرجى زيارة [السماح بالنص النصي المخصص أو منعه.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

