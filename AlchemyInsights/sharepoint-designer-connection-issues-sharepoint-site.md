---
title: مشاكل الاتصال في SharePoint Designer
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
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727158"
---
# <a name="sharepoint-designer-connection-issues"></a>مشاكل الاتصال في SharePoint Designer 

إذا واجه SharePoint Designer مشاكل في الاتصال بمواقع SharePoint ، فالرجاء تجربه الحلول الشائعة التالية.

الخطوة 1: التحقق من تحديث SharePoint Designer 2013 باستخدام [حزمه الخدمة Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) و [2 و 2016 Update ل sharepoint designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



الخطوة 2: مسح ملفات ذاكره التخزين المؤقت المحلية:

1. اغلق SharePoint Designer 2013.

2. علي الكمبيوتر المحلي ، قم بازاله كل الملفات التي تم العثور عليها في كل من المجلدات التالية.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %userprofile%\appdata\local\microsoft\websitecache

3. افتح SharePoint Designer 2013 وادخل الحساب مره أخرى لمعرفه ما إذا كان يعمل.

الخطوة 3: [تمكين المصادقة الحديثة ل Office 2013 علي أجهزه Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

الخطوة 4: سيحتاج المسؤولون إلى **السماح بالبرنامج النصي المخصص** في إعدادات مركز أداره sharepoint للسماح باتصال sharepoint Designer. راجع [السماح بالبرامج النصية المخصصة أو منع](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) المزيد من المعلومات.


