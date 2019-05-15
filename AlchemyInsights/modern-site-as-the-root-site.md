---
title: حديث الموقع الجذر
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057663"
---
# <a name="modern-site-as-root-site"></a>موقع الحديثة كالموقع الجذر

تمكين العملاء [الإصدار الهدف](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) الآن تجربة موقع الاتصالات الحديثة في الموقع الجذر الكلاسيكية للمستأجر SharePoint الخاصة بهم.

يمكن تنشيط هذه الميزة عن طريق تشغيل cmdlet PowerShell بسيطة. على نجاح تنفيذ أوامر PowerShell، سيكون الموقع الجذر لصفحة رئيسية موقع اتصال. تتوفر التفاصيل حول متطلبات PowerShell cmdlet وميزة في المقال [تمكين سبوكومسيتي](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps). 

أننا سوف تدريجيا المتداول هذا، إيقاف تشغيل بشكل افتراضي، للعملاء "الإصدار المستهدف" في أوائل مايو 2019، وطرح ستكون متاحة في جميع أنحاء العالم بنهاية يونيو عام 2019. متابعة للإشارة إلى [مركز](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) لميزات جديدة بحديث. 

**هام**: لا تقم بحذف الموقع الجذر الكلاسيكية لإنشاء "موقع الاتصالات" الحديثة. وهذا غير معتمد من قبل Microsoft. حذف الموقع الجذر سيجعل كافة مواقع SharePoint في المؤسسة الخاصة بك غير متاحة لكافة المستخدمين، حتى يمكنك استعادة الموقع أو إنشاء موقع جديد على نفس العنوان. 
 
 