---
title: تقارير سجل تدقيق SharePoint الكلاسيكية
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068010"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>سجلات تدقيق SharePoint وOneDrive

**سجلات التدقيق الموحدة الحديثة SharePoint وOneDrive من التوافق**

- [تشغيل/إيقاف تشغيل تسجيل التدقيق الموحد](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

لا يوجد تكوين إضافي مطلوب داخل SharePoint أو أندريف.

- استخدم البحث عن تسجيل التدقيق للتحقق من نشاط الملف (الملفات) والمجلد (المجلدات) والمستخدمين والأذونات:

    - [أنشطة الملفات والصفحات](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [أنشطة المجلد](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [أنشطة طلب المشاركة والوصول](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [أنشطة التزامن](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [أنشطة إدارة الموقع](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- لمزيد من المعلومات حول كيفية استرداد هذه الأحداث، راجع [البحث في سجل التدقيق](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).

**سجلات التدقيق الكلاسيكية SharePoint**

لقد قمنا بترحيل التدقيق القديم لـ SPO إلى سجل التدقيق الموحد (UAL). وهذا يعني أساسا أن جميع تقارير التدقيق القديمة SPO سيتم الآن تشغيلها من خلال UAL، وقد تم ترحيل إشارات التدقيق القديمة إلى UAL.

التغييرات الرئيسية:

- التشذيب كقدرة غير متوفرة.
- لا يتوفر القسم الذي تختار فيه أحداث معينة للتدقيق. الرجاء الرجوع إلى [هذا المستند](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) للحصول على قائمة كاملة بالأحداث المدققة المتوفرة بشكل افتراضي.
- الخيار "الموقع" ضمن **التقارير المخصصة** غير متوفر. 
- أحداث "فتح المستندات أو تنزيلها" غير متوفرة. 

