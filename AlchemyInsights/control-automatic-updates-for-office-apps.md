---
title: التحكم في التحديثات التلقائية لتطبيقات Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: f162f11f678e8673d85e52cd9e54cedd7bd6e6a3aee87fcb2731a06d2698ea6a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929868"
---
# <a name="control-automatic-updates-for-office-apps"></a>التحكم في التحديثات التلقائية لتطبيقات Office

بشكل افتراضي، يتم تنزيل Office التطبيقات تلقائيا وتطبيقها في الخلفية دون أي تدخل من قبل المستخدم. ومع ذلك، يمكن للمسؤولين التحكم في كيفية تطبيق التحديثات باستخدام Office التحديث. تسمح إعدادات التحديث للمسؤولين بتمكين التحديثات التلقائية أو  تعطيلها، أو إظهار الزر تحديث الآن أو إخفائه في Office، وتحديد المواعيد النهائية للتحديث، والمزيد. للحصول على معلومات مفصلة، اطلع على الآتي:

- [تكوين إعدادات التحديث Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [التحديث التلقائي Office غير ممكن](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [تعريف كيفية Office بعد تثبيته](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

لمراجعة إعدادات التحديثات الموجودة المطبقة على جهاز عميل، اتبع الخطوات التالية:

1. افتح محرر السجل عن طريق الذهاب إلى **بدء**  >  **تشغيل**  >  **regedit**.
2. قم بالتبديل إلى الموقع التالي وراجع إعدادات Office التحديث:  
    a. HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\  
    b. ClickToRun\Configuration

**ملاحظة**  إذا تم تعيين مفتاح OfficeMgmtCOM، فقد تظهر الرسالة "يتم إدارة التحديثات بواسطة مسؤول النظام" **في** Office الحساب Office  >    >  **التحديثات.** لمزيد من المعلومات، راجع [إدارة التحديثات Microsoft 365 Apps باستخدام Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  