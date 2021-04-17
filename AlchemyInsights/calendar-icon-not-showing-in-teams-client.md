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
ms.openlocfilehash: 6a3f02b69d160c7dce68ed03df59c0d7d1f32f0f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819940"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>عدم ظهور أيقونة "التقويم" في عميل Teams

تتطلب علامة تبويب "التقويم" في Teams إمكانية الوصول إلى علبة بريد Exchange عبر خدمات الويب من Exchange. يمكن أن تكون علبة بريد Exchange عبر الإنترنت أو محلية. بالنسبة للمستخدمين عبر الإنترنت الذين لا يمكنهم رؤية علامة تبويب "التقويم"، تأكد من أنهم [لديهم رخصة علبة بريد Exchange Online وأن علبة البريد ممكّنة](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

إذا كان لدى المستخدم علبة بريد صالحة في Exchange Online، ولكن لا يزال يتعذر عليه رؤية علامة تبويب "التقويم"، فقد تكون المشكلة في الشبكة. استخدم [محلل الاتصال عن بُعد من Microsoft](https://testconnectivity.microsoft.com/) وقم بتشغيل **اختبارات اتصال خدمات الويب من Microsoft Exchange** للمستخدمين المتأثرين.

وأخيراً يمكنك التحقق من [تطبيقات Teams – نُهج إعداد التطبيقات](https://admin.teams.microsoft.com/policies/app-setup) للتأكد من أنه لم تتم إزالة تطبيق التقويم من النهج الذي تم تطبيقه على المستخدم (على الأرجح **العمومي (افتراضي على مستوى المؤسسة)**.

إذا كان المستخدمون يعملون في الأساس محلياً، فأنت بحاجة إلى التأكد من أن "التكوين المختلط" سليم. استخدم["معالج التكوين المختلط"](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent)لاستكشاف الأخطاء وإصلاحها.

تجدر الإشارة إلى أن [Teams يتطلب Exchange 2016 CU3 أو إصدار أحدث](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
