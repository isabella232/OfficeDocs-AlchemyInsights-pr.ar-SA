---
title: مشكلات تسجيل الدخول إلى تطبيقات Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579852"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>إصلاح تطبيقات Microsoft 365 "وحدة النظام الأساسي الموثوق بها للكمبيوتر لا تعمل بشكل صحيح" الرسالة

لإصلاح هذا الخطأ، حاول القيام بالخطوات التالية:

- تثبيت آخر التحديثات [لـ Windows](https://support.microsoft.com/help/4027667/windows-10-update) و [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [مسح بيانات اعتماد Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) باستخدام إدارة بيانات اعتماد Windows.<br/>
    **ملاحظة:** تم تغيير مسارات التسجيل لـ Office 2016 إلى 16.0. (على سبيل: \Software\Microsoft\Office\16.0\Common\Identity\)
- جرّب [عملية استرداد المستخدم](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) لإصلاح فشل وحدة النظام الأساسي الموثوق بها (TPM).
- تعيين EnableADAL = 0 باستخدام الخطوات التالية:  
    1. انقر بزر بدء تشغيل Windows، واختر **تشغيل،** واكتب **regedit،** ثم اختر **موافق**.
    2. حدد **نعم** للسماح لمحرر التسجيل بإجراء تغييرات على جهازك.
    3. في محرر التسجيل، قم بإضافة قيمة DWORD من **EnableADAL** مع إعداد **0** تحت HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

لمزيد من المعلومات، راجع [مشكلات "تسجيل الدخول" في "الاتصال" بعد التحديث إلى Office 2016 بناء 16.0.7967 على Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).