---
title: حذف موقع في SharePoint بشكل دائم
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: f461963c4a5719957258349d667731231023721ab3ee4641538c94371bf3f56d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53944298"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a>حذف موقع في SharePoint بشكل دائم

لإعادة استخدام عنوان URL من موقع محذوف (لإعادة إنشاء موقع)، أو لحذف موقع نهائياً لأنه لم يعد قيد الاستخدام، يمكنك استخدام **حذف نهائياً** من مركز إدارة SharePoint الجديد. 

1. انتقل إلى [صفحة المواقع المحذوفة في مركز إدارة SharePoint الجديد](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) وسجّل الدخول باستخدام حساب يحتوي على أذونات المسؤول لمؤسسك. 

2. من العمود الأيمن، حدد موقعاً. 

3. انقر **حذف بشكل دائم**. 

**ملاحظة**: لا يمكن حذف المواقع المتصلة بالمجموعة نهائياً من مركز إدارة SharePoint الجديد. [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) ستحتاج إلى استخدامه بدلاً من ذلك.  

للحصول على مزيد من المعلومات، اطلع على [حذف موقع نهائياً](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site). 
