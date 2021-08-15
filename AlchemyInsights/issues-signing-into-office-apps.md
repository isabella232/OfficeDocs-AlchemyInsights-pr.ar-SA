---
title: مشاكل في تسجيل الدخول إلى Microsoft 365 التطبيقات
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: b0789a54f48b2850c1dad8651a8209449c805784bea96799f05e67c4bc43fdb0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986878"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>إصلاح رسالة Microsoft 365 "وحدة النظام الأساسي الموثوق بها في الكمبيوتر لا تعمل بشكل صحيح"

لإصلاح هذا الخطأ، حاول القيام بالخطوات التالية:

- قم بتثبيت التحديثات الأخيرة [Windows](https://support.microsoft.com/help/4027667/windows-10-update) [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [مسح Office بيانات الاعتماد](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) باستخدام Windows بيانات الاعتماد.<br/>
    **ملاحظة:** تم تغيير مسارات التسجيل Office 2016 إلى 16.0. (على ما يلي: \Software\Microsoft\Office\16.0\Common\Identity\)
- جرب عملية [استرداد المستخدم](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) لإصلاح حالات فشل وحدة النظام الأساسي الموثوق بها (TPM).
- قم بتعيين EnableADAL = 0 باستخدام الخطوات التالية:  
    1. انقر بزر الماوس الأيمن Windows البدء، واختر **تشغيل**، وا اكتب **regedit**، ثم اختر **موافق**.
    2. حدد **نعم** للسماح لمحرر السجل بإجراء تغييرات على جهازك.
    3. في محرر السجل، أضف قيمة DWORD **من EnableADAL** بإعداد **0** ضمن HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

لمزيد من المعلومات، راجع مشاكل الاتصال في تسجيل الدخول بعد التحديث إلى Office [2016 16.0.7967 على Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).