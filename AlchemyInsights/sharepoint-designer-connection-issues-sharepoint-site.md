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
ms.openlocfilehash: 7451cfe957545537298f57feb5b47bd6d43cddbf
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716879"
---
# <a name="sharepoint-designer-connection-issues"></a>مشكلات الاتصال مصمم SharePoint 

<p>إذا كان SharePoint Designer يواجه مشكلات الاتصال بمواقع SharePoint، الرجاء محاولة الحلول العامة التالية.</p> <p><strong>الخطوة 1:</strong> <strong>يتم تحديث التحقق من "مصمم SharePoint"&nbsp; </strong></p> <ul> <li><a href="https://www.microsoft.com/en-us/download/details.aspx?id=35491">SharePoint Designer 2013</a></li> <li><a href="https://support.microsoft.com/en-us/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1">مصمم SharePoint Service Pack 1 (SP1)</a></li> <li><a href="https://support.microsoft.com/en-us/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721">التحديث الخاص بحزمة SharePoint Designer 2013 (KB3114721)</a></li> </ul> <p><strong>الخطوة 2:</strong> <strong>مسح ملفات ذاكرة التخزين المؤقت المحلية</strong>&nbsp;</p> <ol> <li style="font-weight: 400;">إغلاق 2013 مصمم SharePoint.&nbsp;</li> <li style="font-weight: 400;">على الكمبيوتر المحلي، استعرض المجلدات التالية لإزالة الملفات المخزنة مؤقتاً.&nbsp;</li> <li style="font-weight: 400;">انقر فوق <strong>ابدأ-&gt; تشغيل</strong> وحذف كافة الملفات الموجودة تحت كل من أسفل المواقع.&nbsp;<br /><br />Extensions\Cache خادم %APPDATA%\Microsoft\Web<br />%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache<br />%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</li> <li style="font-weight: 400;">افتح 2013 مصمم SharePoint وأدخل حساب مرة أخرى لمعرفة ما إذا كان يعمل.</li> </ol> <p><strong>الخطوة 3:</strong> <a href="https://docs.microsoft.com/en-us/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=%252fen-us%252farticle%252fEnable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&amp;view=o365-worldwide"> <strong>تمكين مصادقة 2013 Office على Windows الأجهزة الحديثة</strong></a>&nbsp;</p> <p><strong>الخطوة 4:</strong> <strong>سوف يحتاج المسؤولون إلى "السماح لبرنامج نصي مخصص" للسماح باتصال SharePoint Designer</strong>.</p> <p>للحصول على خطوات تفصيلية وأمثلة واعتبارات راجع <a href="https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script">السماح أو منع البرامج النصية المخصصة</a>.&nbsp;</p>


