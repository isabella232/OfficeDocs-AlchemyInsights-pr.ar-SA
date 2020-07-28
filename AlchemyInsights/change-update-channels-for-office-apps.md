---
title: تغيير قنوات التحديث لتطبيقات Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 4939682a6ca95c4f5475ee6aedea48c9ce83df7f
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438700"
---
# <a name="change-update-channels-for-office-apps"></a>تغيير قنوات التحديث لتطبيقات Office

بالنسبة إلى عمليات تثبيت Office الجديدة، استخدم إعدادات تنزيل برامج Office لتحديد قناة التحديث المطلوبة، ثم قم بتثبيت (أو إعادة تثبيت) تطبيقات Office. لمزيد من المعلومات، راجع [إدارة إعدادات تنزيل البرامج في Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365). 

**ملاحظة** يتم تطبيق قناة التحديث المحددة باستخدام إعدادات تحميل برامج Office على كافة المستخدمين الذين يقومون بإجراء عمليات تثبيت جديدة باستخدام المدخل O365. لمزيد من المعلومات، راجع [تنزيل وتثبيت أو إعادة تثبيت Microsoft 365 أو Office 2019 على كمبيوتر شخصي أو Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).   

لتثبيتات Office الموجودة، استخدم أداة نشر Office (ODT) للتبديل إلى قناة تحديث مختلفة:  

1. قم بتنزيل أحدث إصدار من أداة نشر Office (setup.exe) من [مركز تحميل Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
2. حدد اسم القناة التي تريد التبديل إليها. لمزيد من المعلومات، راجع [خيارات التكوين لأداة نشر Office](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).
3. إنشاء ملف XML تكوين تحديد اسم القناة المناسبة، على سبيل المثال، update.xml.  
    (أ) <Configuration>  
    ب. <قناة التحديثات **="شهريا"** />  
    ج. </Configuration>
4. من موجه أوامر مرتفعة، قم بالتبديل إلى موقع المجلد حيث يوجد setup.exe ثم قم بتشغيل الأمر التالي:  
    (أ) setup.exe /تكوين update.xml
5. بدء تشغيل تطبيق Office (مثل Excel)، ثم حدد **حساب ملف**  >  **Account**. في المقطع معلومات المنتج، حدد **تحديث خيارات التحديث**  >  **الآن**.

لمزيد من المعلومات، راجع [كيفية تبديل قنوات التحديث لتطبيقات Office الحالية](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel). 

للتبديل قنوات التحديث لمجموعة محددة من المستخدمين أو باستخدام إدارة التكوين (SCCM) ، تكوين إعداد قناة التحديث باستخدام كائن نهج المجموعة. لمزيد من المعلومات، راجع [نظرة عامة على قنوات التحديث لتطبيقات Microsoft 365](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy). للحصول على تفاصيل، راجع [كيفية إدارة قنوات Office 365 ProPlus لمحترفي تكنولوجيا المعلومات](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) وإدارة [التحديثات إلى تطبيقات Microsoft 365 مع Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).