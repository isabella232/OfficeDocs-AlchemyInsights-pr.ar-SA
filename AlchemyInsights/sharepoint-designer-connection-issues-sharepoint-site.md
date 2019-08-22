---
title: مشكلات الاتصال مصمم SharePoint
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: a4aeaeaea5743c276b907c78317ff30f5610be81
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36508410"
---
# <a name="sharepoint-designer-connection-issues"></a>مشكلات الاتصال مصمم SharePoint 

إذا كان SharePoint Designer يواجه مشكلات الاتصال بمواقع SharePoint، حاول الحلول العامة التالية.

الخطوة 1: التحقق من أنه يتم تحديث 2013 مصمم SharePoint باستخدام [مصمم SharePoint Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) [2 آب/أغسطس عام 2016 تحديث ل 2013 مصمم SharePoint](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



الخطوة 2: مسح ملفات ذاكرة التخزين المؤقت المحلية:

1. إغلاق 2013 مصمم SharePoint.

2. على الكمبيوتر المحلي، بإزالة كافة الملفات الموجودة في كل مجلد من المجلدات التالية.

    - Extensions\Cache خادم %APPDATA%\Microsoft\Web
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. افتح 2013 مصمم SharePoint وأدخل حساب مرة أخرى لمعرفة ما إذا كان يعمل.

الخطوة 3: [تمكين مصادقة 2013 Office على Windows الأجهزة الحديثة](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

الخطوة 4: المسؤولين ستحتاج إلى **السماح لبرنامج نصي مخصص** في إعدادات مركز مسؤول SharePoint للسماح باتصال SharePoint Designer. راجع [السماح أو منع البرامج النصية المخصصة](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) لمزيد من المعلومات.


