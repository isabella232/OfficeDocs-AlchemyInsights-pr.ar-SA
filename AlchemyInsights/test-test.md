---
title: الشروط المفقودة من SharePoint المصطلحات عبر الإنترنت
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: d99458d6f9b65e44ad5945c909b9a8861cf0b1f23463fcdfd5b8351b1c08d670
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54106393"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>تمكين تشفير Bitlocker باستخدام Intune

يمكن استخدام Endpoint Protection Intune لتكوين إعدادات تشفير Boitlocker للأجهزة التي تعمل بنظام Windows كما هو موضح في : إعدادات Windows10 (واللاحقة) لحماية الأجهزة باستخدام Intune

يجب أن تدرك أن العديد من الأجهزة Windows 10 تدعم تشفير bitlocker التلقائي الذي يتم تشغيله بدون تطبيق نهج MDM. قد يؤثر ذلك على تطبيق النهج إذا تم تكوين إعدادات غير افتراضية. راجع الأسئلة الشائعة للحصول على مزيد من التفاصيل.


الأسئلة الشائعة: ما هي إصدارات Windows تشفير أجهزة الدعم باستخدام Endpoint Protection؟
ج: يتم تنفيذ الإعدادات في Intune Endpoint Protection باستخدام Bitlocker CSP.  لا تدعم كل إصدارات أو إصدارات Windows Bitlocker CSP. في الوقت Windows الإصدارات: Enterprise؛ التعليم والجوال و Mobile Enterprise و Professional (من البنية 1809 فصاعدا) معتمدة.




س: إذا كان الجهاز مشفرا بالفعل باستخدام Bitlocker باستخدام الإعدادات الافتراضية ل OS لطريقة التشفير وستطبق قوة التشفير (XTS-AES-128) نهج مع إعدادات مختلفة تلقائيا على إعادة تشفير محرك الأقراص باستخدام الإعدادات الجديدة؟

ج: لا. لتطبيق إعدادات التشفير الجديدة، يجب فك تشفير محرك الأقراص أولا.

ملاحظة بالنسبة للأجهزة التي يتم تسجيلها في Autopilot، لا يتم تشغيل التشفير التلقائي الذي يحدث أثناء OOBE حتى يتم تقييم نهج Intune الذي يسمح باستخدام الإعدادات المستندة إلى النهج في مكان الإعدادات الافتراضية ل OS




س إذا تم تشفير جهاز نتيجة لتطبيق نهج Intune، فهل سيتم فك تشفيره عند إزالة هذا النهج؟

أ: إزالة نهج التشفير ذي الصلة لا يؤدي إلى فك تشفير محركات الأقراص التي تم تكوينها.




س: لماذا يظهر نهج توافق intune أن جهازي لا "تم تمكين Bitlocker" ولكنه كذلك؟

ج: يستخدم الإعداد "تمكين Bitlocker" في نهج التوافق intune عميل Windows حالة الجهاز (DHA). يقيس هذا العميل حالة الجهاز فقط في وقت التشغيل. وبالتالي إذا لم يتم إعادة تشغيل الجهاز منذ اكتمال تشفير bitlocker، فإن خدمة عميل DHA لن تقوم ب الإبلاغ عن bitlocker على أنه نشط.