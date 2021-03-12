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
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743097"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a>تكوين استثناءات MDATP والتحقق من صحتها على جهاز Linux

يمكنك استبعاد بعض الملفات والمجلدات والعمليات والملفات التي تم فتحها من عمليات فحص MDATP. تساعد الاستثناءات على منع الكشف غير الصحيح عن البرامج والملفات الفريدة أو المخصصة لمنظمتك. تساعد الاستثناءات أيضا على الحد من مشاكل الأداء التي تسببها MDATP.

لمعرفة المزيد، راجع [تكوين استثناءات MDATP ل Linux](https://go.microsoft.com/fwlink/?linkid=2144517)والتحقق من صحتها .

> [!IMPORTANT]
> لا تنطبق الاستثناءات الموضحة في هذه المقالة على الإمكانات الأخرى ل MDATP ل Linux، بما في ذلك الكشف عن نقاط النهاية والاستجابة (EDR). يمكن أن تقوم الملفات التي تستبعدها باستخدام الأساليب الموضحة في هذه المقالة بتشغيل تنبيهات EDR وإمكانيات الكشف الأخرى.
