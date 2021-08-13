---
title: استخدام ملفات تعريف البريد الإلكتروني مع Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: b1653b73e7296e7eed411ae73c19342a1187b2eb7e287cff4339ea0ca32d75c1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919410"
---
# <a name="using-email-profiles-with-intune"></a>استخدام ملفات تعريف البريد الإلكتروني مع Intune

يمكن استخدام Intune لإنشاء ملفات تعريف البريد الإلكتروني ونشرها للعميل الأصلي (المضمن) للبريد الإلكتروني على الأنظمة الأساسية للجهاز المتعددة.

للحصول على معلومات حول بعض القيود المقترنة بملفات تعريف البريد الإلكتروني، بما في ذلك كيفية التعامل مع وجود ملفات تعريف موجودة وكيفية إزالة ملفات تعريف البريد الإلكتروني، راجع إضافة إعدادات البريد الإلكتروني إلى الأجهزة التي تستخدم [Intune](https://docs.microsoft.com/intune/email-settings-configure).

لمزيد من المعلومات حول كيفية إنشاء ملفات تعريف البريد الإلكتروني لكل نظام أساسي للجهاز، راجع:

[إعدادات جهاز Android لتكوين البريد الإلكتروني والمصادقة والمزامنة في Intune](https://docs.microsoft.com/intune/email-settings-android)  
[إضافة إعدادات البريد الإلكتروني للأجهزة التي تعمل ب iOS وiPadOS في Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[إعدادات ملف تعريف البريد الإلكتروني في Microsoft Intune للأجهزة التي تعمل Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[إعدادات ملف تعريف البريد الإلكتروني للأجهزة التي تعمل Windows 10 في Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**مشكلة المزامنة الشائعة**

**يمنع ملف تعريف البريد الإلكتروني KNOX على Android جهات اتصال المستخدم والتقويم والمهام من مزامنتها مع أجهزة المستخدمين.**

يوفر ملف تعريف البريد الإلكتروني KNOX على نظام التشغيل Android KNOX للمسؤول خيار تحديد أنواع المحتويات التي تتم مزامنتها مع الجهاز من خلال تعيين كل منها إلى "تمكين".

إذا تم تعيين الإعداد لأي من أنواع المحتويات إلى لم يتم **تكوينه** (الافتراضي)، لن تتم مزامنة نوع المحتوى هذا تلقائيا. قد يقوم المستخدم بتمكين نوع المحتوى الذي يريده مباشرة على الجهاز يدويا، ولكن يتم الكتابة فوق هذا التكوين بواسطة إعداد نهج Intune، وتتوقف المزامنة لنوع المحتوى هذا.

