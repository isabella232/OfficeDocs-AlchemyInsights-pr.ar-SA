---
title: تقارير سجل تدقيق SharePoint الكلاسيكية
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662195"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>سجلات تدقيق SharePoint و OneDrive

## <a name="sharepoint-classic-audit-logs"></a>سجلات التدقيق الكلاسيكية في SharePoint

تم ترحيل تدقيق SPO القديم إلى سجل التدقيق الموحد (أوال). سيتم الآن تشغيل كل تقارير التدقيق القديمة لSPO من خلال أوال ، وتم ترحيل إشارات التدقيق القديمة إلى أوال.

التغييرات الاساسيه:

* لا يتوفر الاقتطاع كامكانيه.
* اختيار الاحداث المحددة للتدقيق غير متوفر. الرجوع إلى [هذا المستند](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) للحصول علي قائمه كامله بالاحداث التدقيق المتوفرة بشكل افتراضي.
* لا يتوفر الخيار " **الموقع** " ضمن " **تقارير مخصصه** ".
* لا يتوفر الخيار **فتح المستندات أو تنزيلها** .

[تكوين إعدادات التدقيق لمجموعه مواقع مشتركه](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>سجلات التدقيق الموحد ل SharePoint و OneDrive الحديثة من التوافق

* [تشغيل ميزه تسجيل التدقيق الموحد](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

لا توجد اي تكوينات اضافيه مطلوبه في SharePoint أو OneDrive.

استخدام ميزه البحث عن تسجيل التدقيق للتحقق من نشاط الملفات والمجلدات ، أو المستخدمين (الأسماء) ، والأذونات:

* [أنشطه الملفات والصفحات](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [أنشطه المجلد](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [أنشطه طلب الوصول والمشاركة](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [أنشطه المزامنة](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [أنشطه أداره الموقع](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

للحصول علي مزيد من المعلومات حول كيفيه استرداد هذه الاحداث ، راجع [البحث في سجل التدقيق](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
