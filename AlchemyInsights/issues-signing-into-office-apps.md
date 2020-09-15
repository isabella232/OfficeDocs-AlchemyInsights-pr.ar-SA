---
title: المشاكل المتعلقة بتسجيل الدخول إلى تطبيقات Microsoft 365
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
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695166"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>إصلاح تطبيقات Microsoft 365 "الوحدة النمطية للنظام الأساسي الموثوق به للكمبيوتر لا تعمل بشكل صحيح"

لإصلاح هذا الخطأ، حاول القيام بالخطوات التالية:

- تثبيت آخر التحديثات ل [Windows](https://support.microsoft.com/help/4027667/windows-10-update) و [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [مسح بيانات اعتماد Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) باستخدام "أداره بيانات اعتماد Windows".<br/>
    **ملاحظه:** لقد تغيرت مسارات التسجيل ل Office 2016 إلى 16.0. (علي سبيل المثال: \Software\Microsoft\Office\16.0\Common\Identity\)
- جرب [عمليه استرداد المستخدم](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) لإصلاح حالات فشل الوحدة النمطية للنظام الأساسي الموثوق به (TPM).
- عين EnableADAL = 0 باستخدام الخطوات التالية:  
    1. انقر بزر الماوس الأيمن فوق "بدء" في Windows ، واختر **تشغيل**، واكتب **regedit**، ثم اختر **موافق**.
    2. حدد **نعم** للسماح لمحرر التسجيل باجراء تغييرات علي جهازك.
    3. في "محرر السجل" ، أضف قيمه DWORD ل **EnableADAL** باستخدام اعداد **0** ضمن HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.

لمزيد من المعلومات ، راجع [مشاكل الاتصال في تسجيل الدخول بعد التحديث إلى Office 2016 16.0.7967 علي Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).