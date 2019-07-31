---
title: مشكلات تسجيل الدخول إلى تطبيقات Office
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
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938120"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>تحديد الرسالة "الوحدة النمطية للنظام الأساسي الموثوق بها للكمبيوتر الخاص بك لا يعمل بشكل صحيح" تطبيقات Office

لإصلاح هذا الخطأ، جرب ما يلي:

- تثبيت التحديثات ل [Windows](https://support.microsoft.com/help/4027667/windows-10-update) و [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- ["مكتب مسح" بيانات الاعتماد](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) باستخدام إدارة بيانات اعتماد Windows.<br/>
    **ملاحظة:** لقد تغيرت المسارات لعام 2016 Office إلى 16.0. (مثلاً: \Software\Microsoft\Office\16.0\Common\Identity\)
- حاول [المستخدم عملية الاسترداد](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) لإصلاح فشل "الوحدة النمطية" النظام الأساسي الموثوق به (TPM).
- تعيين انابليدال = 0 باستخدام الخطوات التالية:  
    1. زر الماوس الأيمن فوق الزر ابدأ في Windows، اختر **تشغيل**، اكتب **regedit**، وثم اختر **"موافق"**.
    2. حدد **نعم** للسماح "محرر التسجيل" لإجراء تغييرات على الجهاز الخاص بك.
    3. في "محرر التسجيل"، إضافة قيمة DWORD **انابليدال** بإعداد **0** تحت HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

لمزيد من المعلومات، راجع [اتصال مشكلات في تسجيل الدخول بعد التحديث إلى عام 2016 Office بناء 16.0.7967 على Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).