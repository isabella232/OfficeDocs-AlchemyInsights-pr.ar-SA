---
title: تكوين تفادي فقدان البيانات على الأجهزة
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402398"
---
# <a name="configure-endpoint-dlp"></a>تكوين تفادي فقدان البيانات على الأجهزة

يسمح لك تفادي فقدان البيانات على الأجهزة من Microsoft بتوسيع حماية تفادي فقدان البيانات وقدرة مراقبة المعلومات الحساسة على أجهزة Windows 10. بعد إلحاق الأجهزة في إدارة الأجهزة، يمكنك إنشاء نُهج DLP لفرض إجراءات الحماية على العناصر. يمكن استخدام مستكشف النشاط لمراقبة نشاط العناصر الحساسة. لمزيد من المعلومات، اطلع على [إلحاق الأجهزة في إدارة الأجهزة](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

لبدء استخدام تفادي فقدان البيانات على الأجهزة:

- تأكد من حصولك على ترخيص SKU/الاشتراكات المناسبة. لمزيد من المعلومات، اطلع على [ترخيص SKU/الاشتراكات](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- تحقق من الأذونات المطلوبة لتمكين إدارة الجهاز أو الوصول إلى صفحة الإلحاق أو تشغيل/إيقاف مراقبة الجهاز. للمزيد من المعلومات، اطلع على [الأذونات](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- قم بإلحاق الأجهزة في إدارة الأجهزة باتباع إجراء إلحاق الأجهزة. إذا فقدت خيار "إلحاق الجهاز" (معاينة) ضمن **إعدادات** توافق M365، فتأكد من أن لديك الترخيص والأذونات المناسبة المشار إليها أعلاه. لمزيد من المعلومات، اطلع على [إلحاق الأجهزة](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- قم بإنشاء نُهج DLP لحماية العناصر الحساسة الخاصة بك. لمزيد من المعلومات، اطلع على [سيناريوهات نهج تفادي فقدان البيانات على الأجهزة](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).

لمزيد من المعلومات حول تفادي فقدان البيانات على الأجهزة من Microsoft، اطلع على [تعرّف على المزيد حول تفادي فقدان البيانات على الأجهزة من Microsoft 365 (معاينة)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**خطوات مهمة لجمع البيانات، إذا كان الدعم مطلوباً:**

1. تنزيل MDATP Client Analyzer Preview من [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")
2. قم بتشغيل الأداة كمسؤول من نافذة cmd:
3. MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t
4. عندما يُطلب منك "إدخال عدد الدقائق لتجميع التتبعات:"، أدخل عدد الدقائق المطلوبة لتشغيل السيناريو
5. تشغيل السيناريو

قم بتجميع إخراج ملف Zip ليتم تسليمه إلى وكيل الدعم.
