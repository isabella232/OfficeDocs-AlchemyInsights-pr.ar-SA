---
title: تعذر إضافة حساب بعد الترقية إلى macOS 11.6 Big Sur
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13840"
- "9008627"
ms.openlocfilehash: 91cb402e63b68de4a08f6dcb80807ff2e01300c9
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506182"
---
# <a name="unable-to-add-an-account-after-upgrading-to-macos-116-big-sur"></a>تعذر إضافة حساب بعد الترقية إلى macOS 11.6 Big Sur

بعد الترقية إلى macOS 11.6، قد لا يظهر حساب OneDrive للعمل أو المدرسة أو حساب OneDrive الشخصي في قائمة الحسابات، وقد لا تتمكن من تسجيل الدخول إلى حساب ثان من التطبيق.

تم تطوير تصحيح لهذه المشكلة. أولا، حدد ما إذا كنت تقوم بتشغيل الإصدار مستقل أو App Store من OneDrive:

- حدد مجموعة OneDrive في شريط القوائم > **تعليمات & الإعدادات**  >  **حول**  >  . إذا لم يتضمن رقم الإصدار **(مستقل)**، لديك إصدار App Store من المنتج.

إذا كنت تستخدم إصدارا مستقلا من OneDrive، فأعاد تشغيل الجهاز، OneDrive التحديثات التلقائية لنسخة حيث تم حل هذه المشكلة. إذا كنت تريد تثبيت النسخة يدويا، ف قم [بتنزيل](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip)ملف.zip هذا، ثم قم ب إلغاء تثبيت الملف، ثم انسخ تطبيق OneDrive إلى مجلد التطبيقات (عن طريق استبدال تطبيق OneDrive الحالي).

إذا كنت تستخدم إصدار App Store، فنظر في تثبيت الإصدار OneDrive. يعمل هذا الإصدار بالطريقة نفسها التي يعمل بها إصدار App Store ولكنه يسمح ل Microsoft بعرض التحديثات بسرعة أكبر للمستخدمين وربطهم بالإصدار الذي يتضمن تصحيحا لهذه المشكلة.

1. قم بتنزيل الإصدار OneDrive [الذي يتضمن تصحيح .](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip)
2. ابدل الملف، وانسخ OneDrive التطبيق إلى مجلد التطبيقات (عن طريق استبدال التطبيق OneDrive الحالي).

إذا كنت بحاجة إلى استخدام إصدار App Store، فانتظر حتى يحرر App Store إصدارا من التطبيق يتضمن الإصلاح. لسوء الحظ، لا تستطيع Microsoft توصيل تاريخ مقدر للإصدار الثابت من متجر التطبيقات.


