---
title: تقارير سجل مراجعة SharePoint الكلاسيكية
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3270f1ab03bacb235cbdc3d710053c858f0a5183
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741952"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>سجلات تدقيق SharePoint وOneDrive

## <a name="sharepoint-classic-audit-logs"></a>سجلات مراجعة الحسابات الكلاسيكية SharePoint

تم ترحيل التدقيق القديم SPO إلى سجل التدقيق الموحد (UAL). وسيتم الآن تشغيل جميع تقارير مراجعة الحسابات القديمة للمنظمات غير القادرة على العمل من خلال UAL، وتم ترحيل إشارات مراجعة الحسابات القديمة إلى UAL.

التغييرات الرئيسية:

* التشذيب غير متوفر كقدرة.
* اختيار أحداث معينة للتدقيق غير متوفر. راجع [هذا المستند](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) للحصول على قائمة كاملة بالأحداث المدققة المتوفرة بشكل افتراضي.
* خيار **الموقع** ضمن **التقارير المخصصة** غير متوفر.
* لا يتوفر خيار **أحداث فتح المستندات أو تنزيلها.**

[تكوين إعدادات التدقيق لمجموعة مواقع](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>سجلات تدقيق اتّحدت SharePoint وOneDrive الحديثة من الامتثال

* [تشغيل/إيقاف تسجيل التدقيق الموحد](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

لا يوجد تكوين إضافي مطلوب داخل SharePoint أو OneDrive.

استخدم بحث تسجيل التدقيق للتحقق من نشاط الملف (الملفات) والمجلد (المجلدات) والمستخدم (الأذونات) والأذونات:

* [أنشطة الملفات والصفحات](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [أنشطة المجلد](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [أنشطة المشاركة وطلب الوصول](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [أنشطة المزامنة](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [أنشطة إدارة الموقع](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

لمزيد من المعلومات حول كيفية استرداد هذه الأحداث، راجع [البحث في سجل التدقيق](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
