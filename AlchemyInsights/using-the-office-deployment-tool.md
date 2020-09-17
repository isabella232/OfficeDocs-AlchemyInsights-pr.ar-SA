---
title: استخدام أداه النشر من Office
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
ms.openlocfilehash: 9698aa12ad73a021a3cc12c8517c1712c48d8385
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794898"
---
# <a name="using-the-office-deployment-tool-odt"></a>استخدام أداه النشر من Office (ODT)

يمكنك استخدام أداه النشر من office (ODT) لنشر إصدارات Office 365 من Office. يتم تشغيل أداه نشر Office (setup.exe) من سطر الأوامر وتستخدم ملف XML تكوين لتحديد الإعدادات التي يجب تطبيقها عند نشر Office.
  
1. قم بتنزيل أحدث إصدار من أداه نشر Office من [مركز التنزيل ل Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. استخدم [أداه تخصيص Office (OCT)](https://config.office.com) لتحديد تفضيلات النشر وإنشاء ملف XML للتكوين. تصدير ملف التكوين ووضعه محليا علي المجلد نفسه الذي يتواجد فيه الsetup.exe.

    **ملاحظه:** تحدث مشاكل تثبيت Office بشكل عام بسبب ملفات تكوين غير صحيحه أو مالفورماتيد. لتجنب هذه المشاكل ، ننصحك باستخدام أداه تخصيص Office لإنشاء ملف التكوين. يمكنك أيضا استيراد ملفات التكوين الموجودة في أداه تخصيص Office.

3. من موجه أوامر غير مقيد ، انتقل إلى الموقع الذي setup.exe فيه وقم بتشغيل أداه نشر Office في وضع التنزيل وحدد ملف التكوين الذي حفظته للتو. في هذا المثال ، يتم تسميه ملف التكوين Configuration.xml:

```setup.exe /download Configuration.xml```

4. قم بتشغيل أداه نشر Office في وضع التكوين وحدد ملف التكوين.

```setup.exe /configure Configuration.xml```

**ملاحظه:** يجب تشغيل هذه الخطوة من الكمبيوتر العميل الذي تريد تثبيت Office عليه ، ويجب ان يكون لديك أذونات المسؤول المحلي علي هذا الكمبيوتر.

للحصول علي مزيد من المعلومات حول استخدام أداه النشر من Office الخاصة بتطبيقات Microsoft 365 لسيناريوهات نشر المؤسسة ، راجع [نظره عامه حول أداه نشر Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). للحصول علي مزيد من التفاصيل حول كيفيه استخدام أداه تخصيص Office ، راجع [نظره عامه حول أداه تخصيص office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
