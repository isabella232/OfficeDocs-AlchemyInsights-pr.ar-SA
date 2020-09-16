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
ms.openlocfilehash: ab3d6e60bc1b67220adbdf7ba61599a6b7aa663a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747763"
---
# <a name="control-automatic-updates-for-office-apps"></a>التحكم في التحديثات التلقائية لتطبيقات Office

بشكل افتراضي ، يتم تنزيل التحديثات الخاصة بتطبيقات Office تلقائيا وتطبيقها في الخلفية بدون تدخل اي مستخدم. ومع ذلك ، يمكن للمسؤولين التحكم في كيفيه تطبيق التحديثات باستخدام إعدادات Office Update. تسمح إعدادات التحديث للمسؤولين بتمكين التحديثات التلقائية أو تعطيلها ، أو إظهار الزر **التحديث الآن** أو إخفاؤه في Office ، وتعيين المواعيد النهائية للتحديث ، والمزيد. للحصول علي معلومات مفصله ، راجع:

- [تكوين إعدادات التحديث ل Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [لم يتم تمكين التحديث التلقائي ل Office](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [تعريف كيفيه تحديث Office بعد تثبيته](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

لمراجعه إعدادات التحديثات الموجودة المطبقة علي جهاز عميل ، اتبع الخطوات التالية:

1. افتح محرر السجل بالانتقال إلى **بدء**  >  **تشغيل**  >  **regedit**.
2. انتقل إلى الموقع التالي وراجع إعدادات تحديث Office:  
    علي. HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft\Office\  
    ب. clicktorun\configuration

**ملاحظه**  إذا تم تعيين المفتاح أوفيسيمجمتكوم ، فقد تري الرسالة "تمت أداره التحديثات بواسطة مسؤول **Office**النظام" في  >  **Account**  >  **تحديثات office**لحساب office. لمزيد من المعلومات ، راجع [أداره التحديثات لتطبيقات microsoft 365 باستخدام أداره تكوين نقاط النهاية من microsoft](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  