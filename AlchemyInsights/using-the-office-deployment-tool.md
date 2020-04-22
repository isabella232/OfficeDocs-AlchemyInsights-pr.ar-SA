---
title: استخدام أداة نشر Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: fa40fef0de9b2e0e1fc329269c24e8bca9ed4146
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726235"
---
# <a name="using-the-office-deployment-tool-odt"></a>استخدام أداة نشر Office (ODT)

يمكنك استخدام أداة نشر Office (ODT) لنشر إصدارات Office 365 من Office. يتم تشغيل أداة نشر Office (setup.exe) من سطر الأوامر وتستخدم ملف XML التكوين لتحديد الإعدادات التي يجب تطبيقها عند نشر Office.
  
1. قم بتنزيل أحدث إصدار من أداة نشر Office من [مركز تنزيل Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. استخدم [أداة تخصيص Office (OCT)](https://config.office.com) لتحديد تفضيلات النشر وإنشاء ملف XML التكوين. تصدير ملف التكوين ووضعه محلياً على نفس المجلد حيث يقيم setup.exe.

    **ملاحظة:** تحدث مشكلات تثبيت Office عادةً بسبب ملفات التكوين التي تم تكوينها بشكل خاطئ أو مالفّنة. لتجنب مثل هذه المشكلات، نوصي باستخدام أداة تخصيص Office لإنشاء ملف التكوين. يمكنك أيضًا استيراد ملفات التكوين الموجودة إلى أداة تخصيص Office.

3. من مطالبة الأمر المرتفعة، قم بالتبديل إلى الموقع الذي يتواجد فيه setup.exe واشغّل أداة نشر Office في وضع التنزيل وحدد ملف التكوين الذي قمت بحفظه للتو. في هذا المثال، يتم تسمية ملف التكوين Configuration.xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. تشغيل أداة نشر Office في وضع التكوين وتحديد ملف التكوين.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **ملاحظة:** يجب تشغيل هذه الخطوة من الكمبيوتر العميل الذي تريد تثبيت Office ويجب أن يكون لديك أذونات المسؤول المحلي على هذا الكمبيوتر.

لمعرفة المزيد حول استخدام أداة نشر Office لتطبيقات Microsoft 365 لسيناريوهات نشر المؤسسة، راجع [نظرة عامة على أداة نشر Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). لمزيد من التفاصيل حول كيفية استخدام أداة تخصيص Office، راجع [نظرة عامة على أداة تخصيص Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
