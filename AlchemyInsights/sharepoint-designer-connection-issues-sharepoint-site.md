---
title: SharePoint مشاكل اتصال المصمم
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: d55f7c1902bb623900fa74bdae70695b6e04ad84ce7b6ea314db614283ec436d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53942012"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint مشاكل اتصال المصمم 

إذا SharePoint "المصمم" مشاكل في الاتصال بالمواقع SharePoint، فالرجاء تجربة الحلول الشائعة التالية.

الخطوة [1:](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) التحقق من تحديث SharePoint Designer 2013 باستخدام SharePoint Designer Service Pack 1 وتحديث 2 أغسطس [2016 ل SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



الخطوة 2: مسح ملفات ذاكرة التخزين المؤقت المحلية:

1. أغلق SharePoint Designer 2013.

2. على الكمبيوتر المحلي، قم بإزالة كل الملفات الموجودة في كل مجلد من المجلدات التالية.

    - ٪APPDATA٪\Microsoft\Web Server Extensions\Cache
    - ٪APPDATA٪\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - ٪USERPROFILE٪\AppData\Local\Microsoft\WebsiteCache

3. افتح SharePoint Designer 2013 وأدخل الحساب مرة أخرى لمعرفة ما إذا كان يعمل.

الخطوة 3: [تمكين المصادقة الحديثة Office 2013 على Windows الأجهزة.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)

الخطوة 4: يجب على  المسؤولين السماح بالنص النصي المخصص في إعدادات SharePoint الإدارة للسماح SharePoint Designer. راجع [السماح بالنص النصي المخصص](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) أو منعه للحصول على مزيد من المعلومات.


