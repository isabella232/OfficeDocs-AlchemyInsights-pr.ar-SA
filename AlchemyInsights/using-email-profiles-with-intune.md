---
title: استخدام ملفات تعريف البريد الإلكتروني مع Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554713"
---
# <a name="using-email-profiles-with-intune"></a>استخدام ملفات تعريف البريد الإلكتروني مع Intune

يمكن استخدام Intune لإنشاء ملفات تعريف البريد الإلكتروني ونشرها لعميل البريد الإلكتروني الأصلي (المدمج) على أنظمة أساسية متعددة للأجهزة.

للحصول على معلومات حول بعض القيود المرتبطة بملفات تعريف البريد الإلكتروني، بما في ذلك كيفية التعامل مع وجود ملفات التعريف الموجودة وكيفية إزالة ملفات تعريف البريد الإلكتروني، راجع [إضافة إعدادات البريد الإلكتروني إلى الأجهزة باستخدام Intune](https://docs.microsoft.com/intune/email-settings-configure).

لمزيد من المعلومات حول كيفية إنشاء ملفات تعريف البريد الإلكتروني لكل نظام أساسي للجهاز، راجع:

[إعدادات جهاز Android لتكوين البريد الإلكتروني والمصادقة والمزامنة في Intune](https://docs.microsoft.com/intune/email-settings-android)  
[إضافة إعدادات البريد الإلكتروني لأجهزة iOS و iPadOS في Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[إعدادات ملف تعريف البريد الإلكتروني في Microsoft Intune للأجهزة التي تعمل بنظام Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[إعدادات ملف تعريف البريد الإلكتروني للأجهزة التي تعمل بنظام التشغيل Windows 10 في Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**مشكلة مزامنة شائعة**

**يمنع ملف تعريف KNOX على البريد الإلكتروني Android جهات اتصال المستخدم والتقويم والمهام من المزامنة مع أجهزة المستخدم.**

يقدم ملف تعريف البريد الإلكتروني لـ KNOX على Android KNOX للمشرف خيار تحديد أنواع المحتوى التي تتم مزامنةها مع الجهاز عن طريق إعداد كل منها على تمكين.

إذا تم تعيين الإعداد لأي من أنواع المحتوى إلى **غير مكوّن** (الافتراضي)، فإن نوع المحتوى هذا غير متزامن تلقائياً. قد يقوم المستخدم بتمكين نوع المحتوى الذي يريده مباشرةً على الجهاز يدوياً، ولكن يتم الكتابة فوق هذا التكوين بواسطة إعداد نهج Intune، وتتوقف المزامنة لنوع المحتوى هذا.

