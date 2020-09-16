---
title: استخدام ملفات تعريف البريد الكتروني مع Intune
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
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653275"
---
# <a name="using-email-profiles-with-intune"></a>استخدام ملفات تعريف البريد الكتروني مع Intune

يمكن استخدام Intune لإنشاء ملفات تعريف البريد الكتروني ونشرها لعميل البريد الكتروني الأصلي (المضمن) علي الانظمه الاساسيه للاجهزه المتعددة.

للحصول علي معلومات حول بعض القيود المقترنة بملفات تعريف البريد الكتروني ، بما في ذلك الطريقة التي تتم بها معالجه ملفات التعريف الموجودة وكيفيه أزاله ملفات تعريف البريد الكتروني ، راجع [أضافه إعدادات البريد الكتروني إلى الاجهزه التي تستخدم Intune](https://docs.microsoft.com/intune/email-settings-configure).

للحصول علي مزيد من المعلومات حول كيفيه إنشاء ملفات تعريف البريد الكتروني لكل نظام أساسي للجهاز ، راجع:

[إعدادات جهاز Android لتكوين البريد الكتروني والمصادقة والمزامنة في Intune](https://docs.microsoft.com/intune/email-settings-android)  
[أضافه إعدادات البريد الكتروني لأجهزه iOS و إيبادوس في Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[إعدادات ملف تعريف البريد الكتروني في Microsoft Intune للاجهزه التي تعمل بنظام Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[إعدادات ملف تعريف البريد الكتروني للاجهزه التي تعمل بنظام Windows 10 في Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**مشكله المزامنة الشائعة**

**يحول كنوكس علي ملف تعريف البريد الكتروني لنظام التشغيل Android جات اتصال المستخدم والتقويم والمهام ، من المزامنة إلى أجهزه المستخدم.**

يعرض كنوكس علي ملف تعريف البريد الكتروني الذي يعمل بنظام التشغيل Android كنوكس المسؤول خيارا لتحديد أنواع المحتويات التي ستتم مزامنتها علي الجهاز بتعيين كل إلى تمكين.

إذا تم تعيين الاعداد لأي نوع من أنواع المحتويات إلى **غير مكون** (الافتراضي) ، فلن تتم مزامنة نوع المحتوي هذا تلقائيا. قد يقوم المستخدم بتمكين نوع المحتوي الذي يريدونه مباشره علي الجهاز يدويا ، ولكن يتم الكتابة فوق هذا التكوين بواسطة اعداد نهج Intune ، وتتوقف المزامنة عن نوع المحتوي هذا.

