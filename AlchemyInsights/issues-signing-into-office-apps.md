---
title: مشاكل تسجيل الدخول إلى تطبيقات Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709093"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>إصلاح رسالة تطبيقات Microsoft 365 "الوحدة النمطية ل "النظام الأساسي الموثوق به" على الكمبيوتر لا تعمل بشكل صحيح

لإصلاح هذا الخطأ، حاول القيام بالخطوات التالية:

- تثبيت آخر التحديثات [لنظامي التشغيل Windows](https://support.microsoft.com/help/4027667/windows-10-update) و [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [مسح بيانات اعتماد Office](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) باستخدام إدارة بيانات اعتماد Windows.<br/>
    **ملاحظة:** تم تغيير مسارات التسجيل ل Office 2016 إلى 16.0. (على Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- جرب عملية [استرداد المستخدم لإصلاح](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) حالات فشل الوحدة النمطية (TPM) الموثوق بها في النظام الأساسي.
- قم بتعيين EnableADAL = 0 باستخدام الخطوات التالية:  
    1. انقر بزر الماوس الأيمن فوق الزر "ابدأ" في Windows، واختر **"تشغيل"،** ثم اكتب **regedit،** ثم اختر **"موافق".**
    2. حدد **"نعم"** للسماح ل "محرر السجل" بإجراء تغييرات على جهازك.
    3. في "محرر السجل"، أضف قيمة DWORD ل **EnableADAL** بإعداد **0** ضمن HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

لمزيد من المعلومات، راجع مشاكل الاتصال في تسجيل الدخول بعد التحديث إلى [Office 2016 إصدار 16.0.7967 على Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)