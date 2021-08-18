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
ms.openlocfilehash: 97a8d4e7db9aac65e6a505c0bef8b41d2ea23353
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323905"
---
# <a name="configure-endpoint-dlp"></a>تكوين تفادي فقدان البيانات على الأجهزة

يسمح لك تفادي فقدان البيانات على الأجهزة من Microsoft بتوسيع حماية تفادي فقدان البيانات وقدرة مراقبة المعلومات الحساسة على أجهزة Windows 10. بعد إلحاق الأجهزة في إدارة الأجهزة، يمكنك إنشاء نُهج DLP لفرض إجراءات الحماية على العناصر. يمكن استخدام مستكشف النشاط لمراقبة نشاط العناصر الحساسة. لمزيد من المعلومات، اطلع على [إلحاق الأجهزة في إدارة الأجهزة](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

لبدء استخدام تفادي فقدان البيانات على الأجهزة:

- تأكد من حصولك على ترخيص SKU/الاشتراكات المناسبة. لمزيد من المعلومات، اطلع على [ترخيص SKU/الاشتراكات](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- تحقق من الأذونات المطلوبة لتمكين إدارة الجهاز أو الوصول إلى صفحة الإلحاق أو تشغيل/إيقاف مراقبة الجهاز. للمزيد من المعلومات، اطلع على [الأذونات](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- قم بإلحاق الأجهزة في إدارة الأجهزة باتباع إجراء إلحاق الأجهزة. لمزيد من المعلومات، اطلع على [إلحاق الأجهزة](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- قم بإنشاء نُهج DLP لحماية العناصر الحساسة الخاصة بك. لمزيد من المعلومات، اطلع على [سيناريوهات نهج تفادي فقدان البيانات على الأجهزة](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

لمزيد من المعلومات حول تفادي فقدان البيانات على الأجهزة من Microsoft، اطلع على [تعرّف على المزيد حول تفادي فقدان البيانات على الأجهزة من Microsoft 365 (معاينة)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**خطوات مهمة لجمع البيانات، إذا كان الدعم مطلوباً:**

1. تنزيل معاينة محلل عميل [MDATP](https://aka.ms/betamdatpanalyzer).
1. قم بتشغيل الأداة كمسؤول من نافذة cmd:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. عند مطالبتك بإدخال **عدد الدقائق** لتجميع التتبعات: ، أدخل عدد الدقائق المطلوبة لتشغيل السيناريو.
1. تشغيل السيناريو.

جمع إخراج ملف Zip لتقديمه إلى وكيل الدعم.
