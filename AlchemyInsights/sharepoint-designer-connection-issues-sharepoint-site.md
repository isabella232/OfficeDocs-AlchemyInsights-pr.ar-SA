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
ms.openlocfilehash: 9730bd66afd494385db3de605f5fe68d0f274ed3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051700"
---
# <a name="sharepoint-designer-connection-issues"></a>مشكلات اتصال مصمم SharePoint 

إذا كان مصمم SharePoint يواجه مشكلات في الاتصال بمواقع SharePoint ، الرجاء محاولة الحلول الشائعة التالية.

الخطوة 1: تحقق من ان يتم تحديث SharePoint Designer 2013 مع [Sharepoint مصمم الخدمة Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) و [2 أغسطس 2016 تحديث ل sharepoint designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



الخطوة 2: مسح ملفات ذاكره التخزين المؤقت المحلية:

1. إغلاق SharePoint Designer 2013.

2. علي الكمبيوتر المحلي ، قم بازاله كافة الملفات الموجودة في كل من المجلدات التالية.

    - %Appdate%\tegs\micscatortontetes\ التخزين المؤقت
    - %Appdata%\tedsdesigner\proxyassemblycache \ SharePoint
    - %Userprofile%\appdates\locics\mics\websitecache

3. فتح SharePoint Designer 2013 وادخل الحساب مره أخرى لمعرفه ما إذا كان يعمل.

الخطوة 3: [تمكين المصادقة الحديثة ل Office 2013 علي أجهزه Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

الخطوة 4: سيحتاج المسؤولون إلى **السماح بالبرنامج النصي المخصص** في إعدادات مركز مسؤول sharepoint للسماح باتصال مصمم sharepoint. راجع [السماح بالبرنامج النصي المخصص أو منعه](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) للحصول علي مزيد من المعلومات.


