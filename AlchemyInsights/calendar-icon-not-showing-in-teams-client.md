---
title: عدم ظهور أيقونة "التقويم" في عميل Teams
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
- "9001219"
- "4375"
ms.openlocfilehash: 7881d6837cb7d99180d2cc1b28d327ce12e4b836d33e4fca099569d4f72510fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989578"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>عدم ظهور أيقونة "التقويم" في عميل Teams

تتطلب علامة تبويب "التقويم" في Teams إمكانية الوصول إلى علبة بريد Exchange عبر خدمات الويب من Exchange. يمكن أن تكون علبة بريد Exchange عبر الإنترنت أو محلية. بالنسبة للمستخدمين عبر الإنترنت الذين لا يمكنهم رؤية علامة تبويب "التقويم"، تأكد من أنهم [لديهم رخصة علبة بريد Exchange Online وأن علبة البريد ممكّنة](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

إذا كان لدى المستخدم علبة بريد صالحة في Exchange Online، ولكن لا يزال يتعذر عليه رؤية علامة تبويب "التقويم"، فقد تكون المشكلة في الشبكة. استخدم [محلل الاتصال عن بُعد من Microsoft](https://testconnectivity.microsoft.com/) وقم بتشغيل **اختبارات اتصال خدمات الويب من Microsoft Exchange** للمستخدمين المتأثرين.

وأخيراً يمكنك التحقق من [تطبيقات Teams – نُهج إعداد التطبيقات](https://admin.teams.microsoft.com/policies/app-setup) للتأكد من أنه لم تتم إزالة تطبيق التقويم من النهج الذي تم تطبيقه على المستخدم (على الأرجح **العمومي (افتراضي على مستوى المؤسسة)**.

إذا كان المستخدمون يعملون في الأساس محلياً، فأنت بحاجة إلى التأكد من أن "التكوين المختلط" سليم. استخدم["معالج التكوين المختلط"](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent)لاستكشاف الأخطاء وإصلاحها.

تجدر الإشارة إلى أن [Teams يتطلب Exchange 2016 CU3 أو إصدار أحدث](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
