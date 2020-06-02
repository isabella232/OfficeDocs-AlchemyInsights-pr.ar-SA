---
title: مشكلات اتصال مصمم SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511531"
---
# <a name="sharepoint-designer-connection-issues"></a>مشكلات اتصال مصمم SharePoint 

إذا كان SharePoint Designer يواجه مشكلات في الاتصال بمواقع SharePoint، فيرجى تجربة الحلول الشائعة التالية.

الخطوة 1: تحقق من تحديث SharePoint Designer 2013 باستخدام [حزمة خدمة مصمم SharePoint 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) وتحديث 2 [أغسطس 2016 لمصمم SharePoint 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



الخطوة 2: مسح ملفات ذاكرة التخزين المؤقت المحلية:

1. إغلاق SharePoint مصمم 2013.

2. على الكمبيوتر المحلي، قم بإزالة كافة الملفات الموجودة في كل من المجلدات التالية.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint مصمم\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. افتح SharePoint Designer 2013 وأدخل الحساب مرة أخرى لمعرفة ما إذا كان يعمل.

الخطوة 3: [تمكين المصادقة الحديثة لـ Office 2013 على أجهزة Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

الخطوة 4: سيحتاج المسؤولون إلى **السماح بالبرنامج النصي المخصص** في إعدادات مركز مسؤول SharePoint للسماح باتصال مصمم SharePoint. راجع [السماح بالبرنامج النصي المخصص أو منعه](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) للحصول على مزيد من المعلومات.


