---
title: استخدام أداة Office النشر
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 39a011d4b121492d222ff620e70d9860231b7bcfe0d7fd2ecfd93de1ef502f5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083757"
---
# <a name="using-the-office-deployment-tool-odt"></a>استخدام أداة Office (ODT)

يمكنك استخدام أداة Office (ODT) لنشر Office 365 من Office. يتم Office أداة النشر (setup.exe) من سطر الأوامر وتستخدم ملف تكوين XML لتحديد الإعدادات التي يجب تطبيقها عند نشر Office.
  
1. قم بتنزيل أحدث إصدار من أداة Office من [مركز تنزيل Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. استخدم أداة [Office التخصيص (OCT)](https://config.office.com) لتحديد تفضيلات النشر وإنشاء ملف تكوين XML. تصدير ملف التكوين ثم ضعه محليا على المجلد نفسه الذي setup.exe فيه.

    **ملاحظة:** Office عادة ما تحدث مشاكل التثبيت بسبب ملفات التكوين التي تم تكوينها بشكل غير صحيح أو التي تم تكوينها بشكل غير صحيح. لتجنب مثل هذه المشاكل، نوصي باستخدام أداة Office التخصيص لإنشاء ملف التكوين. يمكنك أيضا استيراد ملفات التكوين الموجودة إلى Office التخصيص.

3. من موجه أوامر غير مرفأ، قم بالتبديل إلى الموقع الذي setup.exe فيه وتشغيل أداة النشر Office في وضع التنزيل وحدد ملف التكوين الذي حفظته للتو. في هذا المثال، يسمى ملف التكوين Configuration.xml:

```setup.exe /download Configuration.xml```

4.قم بتشغيل Office النشر في وضع التكوين وحدد ملف التكوين.

```setup.exe /configure Configuration.xml```

**ملاحظة:** يجب تشغيل هذه الخطوة من الكمبيوتر العميل الذي تريد تثبيت Office عليه ويجب أن يكون لديك أذونات المسؤول المحلي على هذا الكمبيوتر.

لمعرفة المزيد حول استخدام أداة Office لسيناريوهات النشر Microsoft 365 Apps for enterprise، راجع نظرة عامة على Office [النشر.](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool) لمزيد من التفاصيل حول كيفية استخدام أداة Office التخصيص، راجع نظرة عامة [على Office التخصيص.](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)
