---
title: باستخدام أداة نشر Office
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: c7e0e96f225030590fdd516eaf3115c93a6335b6
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29898633"
---
# <a name="using-the-office-deployment-tool-odt"></a>باستخدام أداة نشر Office (ODT)

يمكنك استخدام أداة نشر Office (ODT) لنشر إصدارات Office 365 من Office. أداة نشر Office (setup.exe) من سطر الأوامر ويستخدم ملف تكوين XML لتحديد الإعدادات لتطبيق مستندات Office.
  
1. تنزيل أحدث إصدار من "الأداة Office النشر" من ["مركز تحميل microsoft"](http://go.microsoft.com/fwlink/p/?LinkID=626065).
    
2. استخدام [أداة تخصيص Office (OCT)](https://config.office.com) لتحديد تفضيلات التوزيع وإنشاء ملف تكوين XML. تصدير ملف التكوين ووضعه محلياً في نفس المجلد حيث يوجد setup.exe. 
    
    **ملاحظة:** عادة ما تحدث مشكلات المستحقة لصحيح تثبيت office أو ملفات التكوين مالفورماتيد. لتجنب مثل هذه المشكلات، نوصي باستخدام "أداة تخصيص Office" لإنشاء ملف التكوين. يمكنك أيضا استيراد ملفات التكوين الموجودة في أداة تخصيص Office. 
    
3. من موجه أوامر غير مقيد، قم بالتبديل إلى المجلد حيث يوجد setup.exe وتشغيل أداة نشر Office في وضع الخطوط وتحديد ملف التكوين الذي قمت بحفظه. في هذا المثال، يتم تسمية ملف التكوين Configuration.xml:
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. تشغيل أداة نشر Office في تكوين وضع وحدد ملف التكوين.
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **ملاحظة:** يجب تشغيل هذه الخطوة من جهاز الكمبيوتر العميل الذي تريد تثبيت Office ويجب أن يكون لديك أذونات المسؤول المحلية على هذا الكمبيوتر. 
    
لمزيد من المعلومات حول استخدام أداة نشر Office لسيناريوهات النشر Office 365 ProPlus، راجع [نظرة عامة حول أداة نشر Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). للحصول على مزيد من التفاصيل حول كيفية استخدام أداة تخصيص Office، راجع [نظرة عامة حول أداة تخصيص Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
  

