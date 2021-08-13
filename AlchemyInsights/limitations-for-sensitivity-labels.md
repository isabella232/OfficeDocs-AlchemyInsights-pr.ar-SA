---
title: قيود تسميات الحساسية لملفات Office في SharePoint OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12451"
- "9000181"
ms.openlocfilehash: e197c43712c0ead9508a1cfdf48b51d01d2ae957649f73703f9c33733e332bf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813148"
---
# <a name="limitations-for-sensitivity-labels-for-office-files-in-sharepoint-and-onedrive"></a>قيود تسميات الحساسية لملفات Office في SharePoint OneDrive

عند تمكين تسميات الحساسية لملفات Office في SharePoint OneDrive، كن على علم بالمتطلبات والحدود، والتي تتضمن:

- SharePoint أو OneDrive معالجة بعض الملفات التي تم تسميتها وتشفيرها من تطبيقات سطح المكتب Office عندما تحتوي الملفات على بيانات PowerQuery أو بيانات مخزنة بواسطة الوظائف الإضافية المخصصة أو أجزاء XML مخصصة.
- SharePoint أو OneDrive تطبيق تسميات الحساسية تلقائيا على الملفات الموجودة التي قمت بالفعل بتشفيرها باستخدام تسميات Azure Information Protection (AIP). لتطبيق تسميات الحساسية على الملفات المشفرة: 
    - تأكد من ترحيل تسميات AIP ونشرها إلى Microsoft 365 التوافق.
    - قم بتنزيل الملفات الملصقات، ثم قم بتحميلها إلى موقعها الأصلي SharePoint أو OneDrive الأصلي.
- بالنسبة للمستندات المشفرة، الطباعة غير معتمدة.

للحصول على تفاصيل إضافية حول القيود، راجع تمكين تسميات الحساسية لملفات Office في SharePoint [OneDrive](/microsoft-365/compliance/sensitivity-labels-sharepoint-onedrive-files#limitations).
