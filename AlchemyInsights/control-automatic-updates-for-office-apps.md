---
title: التحكم في التحديثات التلقائية لتطبيقات Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438692"
---
# <a name="control-automatic-updates-for-office-apps"></a>التحكم في التحديثات التلقائية لتطبيقات Office

يتم بشكل افتراضي تنزيل تحديثات تطبيقات Office تلقائياً وتطبيقها في الخلفية دون أي تدخل من المستخدم. ومع ذلك، يمكن للمسؤولين التحكم في كيفية تطبيق التحديثات باستخدام إعدادات Office Update. تسمح إعدادات التحديث للمسؤولين بتمكين التحديثات التلقائية أو تعطيلها، وإظهار الزر **Update Now** في Office أو إخفائه، وتعيين المواعيد النهائية للتحديث، وغير ذلك الكثير. للحصول على معلومات مفصلة، انظر:

- [تكوين إعدادات التحديث لـ Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [لم يتم تمكين التحديث التلقائي لـ Office](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [تحديد كيفية تحديث Office بعد تثبيته](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

لمراجعة إعدادات التحديثات الموجودة المطبقة على جهاز عميل، اتبع الخطوات التالية:

1. فتح محرر التسجيل بواسطة الانتقال إلى **بدء**  >  **تشغيل**  >  **regedit**.
2. التبديل إلى الموقع التالي ومراجعة إعدادات Office Update:  
    (أ) HKEY_LOCAL_MACHINE\SOFTWARE\\مايكروسوفت\Office\  
    ب. انقر فوق التشغيل\تكوين

**ملاحظة**  إذا تم تعيين مفتاح OfficeMgmtCOM، قد ترى رسالة "يتم إدارة التحديثات من قبل مسؤول النظام الخاص بك" في تحديثات Office **Office**  >  **حساب**  >  **Office**. لمزيد من المعلومات، راجع [إدارة التحديثات إلى تطبيقات Microsoft 365 مع إدارة تكوين نقطة النهاية ل Microsoft](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  