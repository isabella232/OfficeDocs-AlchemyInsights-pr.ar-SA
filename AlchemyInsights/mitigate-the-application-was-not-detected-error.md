---
title: الحد من حدوث خطأ عدم الكشف عن التطبيق
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: 34b2024257c88512db170cbb0e672c1628ad8e3935342f87c5032492e1ad0259
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54026101"
---
# <a name="mitigate-the-application-was-not-detected-error"></a>الحد من حدوث خطأ "لم يتم الكشف عن التطبيق"

يحدث خطأ تثبيت التطبيق "لم يتم الكشف عن التطبيق بعد اكتمال التثبيت بنجاح"، والذي يتم الإبلاغ عنه بواسطة Intune، وقد يحدث في جميع أنظمة التشغيل الأساسية (Windows وiOS وAndroid).

السيناريوهات الأكثر شيوعاً التي تؤدي إلى حدوث هذا الخطأ:

- تحديث التطبيق خارج Intune (من متجر تطبيقات تابع لجهة خارجية) بعد النشر الأولي. على سبيل المثال، قد تقوم بعض التطبيقات مثل Google Chrome بإجراء تحديثات تلقائية.
- قام أحد المستخدمين بإزالة تثبيت التطبيق بعد التثبيت الأولي.

للحد من هذه المشكلة، قم أولاً بمراجعة الأجهزة التي تأثرت لتحديد السيناريو الذي يحدث فيه الخطأ.

- إذا تم تحديث التطبيق خارج Intune، يمكن تعيين نشر التطبيق بحيث يتجاهل إصدار التطبيق. للقيام بذلك، ضمن **تكوين التطبيق > معلومات التطبيق**، قم بتعيين **تجاهل إصدار التطبيق** إلى **نعم**.
- عند استهداف العميل، قد يكون من المناسب نشر التطبيق بوصفه "مطلوب"، والتأكد من نشر الإصدار الأخير.
- بدلاً من ذلك، يمكن على النظام الأساسي iOS، استخدام وظيفة **التحديث التلقائي** المقترنة ببرنامج الشراء المجمع من Apple، والذي يمكن تكوينه ليتم التحديث تلقائياً إلى إصدارات التطبيق الحديثة بمجرد توفرها.

للحصول على المزيد من المعلومات حول استكشاف مشكلات تثبيت التطبيقات وإصلاحها، الرجاء مراجعة [استكشاف مشكلات تثبيت التطبيقات وإصلاحها](https://docs.microsoft.com/intune/troubleshoot-app-install).
