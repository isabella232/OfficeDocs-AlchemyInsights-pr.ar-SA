---
title: كيف لاستيراد-nk2-الملفات
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: 83d30b2d62908db791f21ec5ed7fd5537e7a0944
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759319"
---
# <a name="how-to-import-nk2-files"></a>كيفية استيراد ملفات .nk2 

عند بدء تشغيل Microsoft Outlook 2013 أو Outlook 2016 أو Outlook 2019 أو Outlook for Microsoft 365 للمرة الأولى، يتم استيراد ذاكرة التخزين المؤقت للكنية (المخزنة في ملف *اسم الملف الشخصي*.nk2) إلى رسالة مخفية في مخزن الرسائل الافتراضي.

لاستيراد ملفات .nk2 إلى Outlook 2013 أو Outlook 2016 أو Outlook 2019 أو Outlook for Microsoft 365، تأكد من أن ملف .nk2 موجود في المجلد التالي: %appdata%\Microsoft\Outlook

**ملاحظة:** يجب أن يكون لملف .nk2 نفس اسم ملف Outlook 2013 الحالي أو ملف Outlook 2016. بشكل افتراضي، اسم ملف التعريف هو "Outlook". للتحقق من اسم الملف الشخصي، اتبع الخطوات التالية: 
1. انقر فوق **ابدأ،** ثم انقر فوق **لوحة التحكم**.
2. انقر نقراً مزدوجاً على **البريد**.
3. في مربع حوار إعداد البريد، حدد **إظهار الملفات الشخصية**.
4. حدد **بدء** > **التشغيل**.
5. في المربع **المفتوح،** اكتب *outlook.exe /importnk2،* ثم حدد **موافق**. 

بعد استيراد ملف .nk2، يتم دمج محتويات الملف في ذاكرة التخزين المؤقت اللقب الموجودة المخزنة في علبة البريد الخاصة بك.

**ملاحظة:** تتم إعادة تسمية ملف .nk2 مع ملحق اسم ملف .old في المرة التالية التي تبدأ Outlook 2013 أو Outlook 2016 أو Outlook 2019 أو Outlook for Microsoft 365. إذا كنت ترغب في إعادة استيراد ملف .nk2، قم بإزالة ملحق اسم الملف القديم أولاً.

لمزيد من المعلومات، راجع [استيراد قائمة الإكمال التلقائي أو نسخها إلى كمبيوتر آخر](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).