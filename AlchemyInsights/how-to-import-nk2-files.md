---
title: كيفيه الاستيراد-nk2 الملفات
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: 6a823f6e0c4c46de64dd7b70fb40c76255d78ec1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780046"
---
# <a name="how-to-import-nk2-files"></a>كيفيه استيراد ملفات nk2 

عند بدء تشغيل Microsoft Outlook 2013 أو Outlook 2016 أو Outlook 2019 أو Outlook for Microsoft 365 للمرة الاولي ، يتم استيراد ذاكره التخزين المؤقت لكنية (المخزنة في الملف *profilename*nk2) إلى رسالة مخفيه في مخزن الرسائل الافتراضي.

لاستيراد ملفات nk2 إلى Outlook 2013 أو Outlook 2016 أو Outlook 2019 أو Outlook for Microsoft 365 ، تاكد من ان ملف nk2 موجود في المجلد التالي:%appdata%\Microsoft\Outlook

**ملاحظه**: يجب ان يكون لملف nk2 اسم ملف تعريف outlook 2013 أو outlook 2016 الحالي. بشكل افتراضي ، يكون اسم التشكيل الجانبي هو "Outlook." للتحقق من اسم ملف التعريف ، اتبع الخطوات التالية: 
1. انقر فوق **أبدا**، ثم فوق **لوحه التحكم**.
2. انقر نقرا مزدوجا فوق **البريد**.
3. في مربع الحوار اعداد البريد ، حدد **إظهار ملفات التعريف**.
4. حدد **بدء**  >  **التشغيل**.
5. في المربع **فتح** ، اكتب *outlook.exe/importnk2*، ثم حدد **موافق**. 

بعد استيراد الملف nk2 ، يتم دمج محتويات الملف في ذاكره التخزين المؤقت لكنية الموجودة المخزنة في علبه البريد.

**ملاحظه**: يتم أعاده تسميه ملف nk2 باستخدام ملحق اسم الملف القديم في المرة التالية التي تقوم فيها بتشغيل outlook 2013 أو outlook 2016 أو outlook 2019 أو Outlook ل Microsoft 365. إذا أردت أعاده استيراد ملف nk2 ، فقم بازاله ملحق اسم الملف القديم أولا.

لمزيد من المعلومات ، راجع [استيراد قائمه الإكمال التلقائي أو نسخها إلى كمبيوتر آخر](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).