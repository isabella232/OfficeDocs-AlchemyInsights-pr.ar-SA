---
title: مستويات إذن SharePoint على الإنترنت
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760680"
---
# <a name="sharepoint-designer-connection-issues"></a>مشكلات الاتصال مصمم SharePoint 

إذا كان SharePoint Designer يواجه مشكلات الاتصال بمواقع SharePoint، الرجاء محاولة الحلول العامة التالية.

الخطوة 1: التحقق من تحديث "مصمم SharePoint".

- [SharePoint Designer 2013](https://www.microsoft.com/download/details.aspx?id=35491)

- [مصمم SharePoint Service Pack 1 (SP1)](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [التحديث الخاص بحزمة SharePoint Designer 2013 (KB3114721)](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

الخطوة 2: مسح ملفات ذاكرة التخزين المؤقت المحلية

- إغلاق 2013 مصمم SharePoint.

- على الكمبيوتر المحلي، استعرض المجلدات التالية لإزالة الملفات المخزنة مؤقتاً.

- انقر فوق ابدأ، تشغيل وحذف كافة الملفات التي تم العثور على تحت كل من أسفل المواقع.

خادم %APPDATA%\Microsoft\Web Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

افتح 2013 مصمم SharePoint وأدخل حساب مرة أخرى لمعرفة ما إذا كان يعمل.

الخطوة 3: [تمكين مصادقة 2013 Office على Windows الأجهزة الحديثة](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)

الخطوة 4: سيحتاج المسؤولين "السماح للبرامج النصية المخصصة" للسماح باتصال SharePoint Designer.

للحصول على خطوات تفصيلية وأمثلة واعتبارات راجع [السماح أو منع البرامج النصية المخصصة](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


