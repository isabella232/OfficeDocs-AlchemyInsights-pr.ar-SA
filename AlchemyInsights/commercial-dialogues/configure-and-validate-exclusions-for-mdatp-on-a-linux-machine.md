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
ms.openlocfilehash: 96579b28923e392a0fa05c56833fed1b45eb118437ac7e8333c610ed69126f8e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53916402"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a>تكوين استثناءات MDATP والتحقق من صحتها على جهاز Linux

يمكنك استبعاد بعض الملفات والمجلدات والعمليات والملفات التي تم فتحها من عمليات فحص MDATP. تساعد الاستثناءات على منع الكشف غير الصحيح عن البرامج والملفات الفريدة أو المخصصة لمنظمتك. تساعد الاستثناءات أيضا على الحد من مشاكل الأداء التي تسببها MDATP.

لمعرفة المزيد، راجع [تكوين استثناءات MDATP ل Linux](https://go.microsoft.com/fwlink/?linkid=2144517)والتحقق من صحتها .

> [!IMPORTANT]
> لا تنطبق الاستثناءات الموضحة في هذه المقالة على الإمكانات الأخرى ل MDATP ل Linux، بما في ذلك الكشف عن تهديدات نقاط النهاية والرد عليها (الكشف التلقائي والاستجابة على النقط النهائية). لا يزال بإمكانك تشغيل الملفات التي تستبعدها باستخدام الأساليب الموضحة في هذه المقالة الكشف التلقائي والاستجابة على النقط النهائية التنبيهات وإمكانيات الكشف الأخرى.
