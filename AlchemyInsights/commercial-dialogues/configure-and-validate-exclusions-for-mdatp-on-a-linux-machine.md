---
title: تكوين استثناءات MDATP والتحقق من صحتها على جهاز Linux
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: b2487e283f37498539bfac0583ef7e21d1817db0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321272"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a>تكوين استثناءات MDATP والتحقق من صحتها على جهاز Linux

يمكنك استبعاد بعض الملفات والمجلدات والعمليات والملفات التي تم فتحها من عمليات فحص MDATP. تساعد الاستثناءات على منع الكشف غير الصحيح عن البرامج والملفات الفريدة أو المخصصة لمنظمتك. تساعد الاستثناءات أيضا على الحد من مشاكل الأداء التي تسببها MDATP.

لمعرفة المزيد، راجع [تكوين استثناءات MDATP ل Linux](https://go.microsoft.com/fwlink/?linkid=2144517)والتحقق من صحتها .

**هام:** لا تنطبق الاستثناءات الموضحة في هذه المقالة على الإمكانات الأخرى ل MDATP ل Linux، بما في ذلك الكشف عن تهديدات نقاط النهاية والرد عليها (الكشف التلقائي والاستجابة على النقط النهائية). لا يزال بإمكانك تشغيل الملفات التي تستبعدها باستخدام الأساليب الموضحة في هذه المقالة الكشف التلقائي والاستجابة على النقط النهائية التنبيهات وإمكانيات الكشف الأخرى.
