---
title: عدم ظهور أيقونة "التقويم" في عميل Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 21692639fb746b2e5aab3dfc8894293d5dc890ac
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931778"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>عدم ظهور أيقونة "التقويم" في عميل Teams

تتطلب علامة تبويب "التقويم" في Teams إمكانية الوصول إلى علبة بريد Exchange عبر خدمات الويب من Exchange. يمكن أن تكون علبة بريد Exchange عبر الإنترنت أو محلية. بالنسبة للمستخدمين عبر الإنترنت الذين لا يمكنهم رؤية علامة تبويب "التقويم"، تأكد من أنهم [لديهم رخصة علبة بريد Exchange Online وأن علبة البريد ممكّنة](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

إذا كان لدى المستخدم علبة بريد صالحة في Exchange Online، ولكن لا يزال يتعذر عليه رؤية علامة تبويب "التقويم"، فقد تكون المشكلة في الشبكة. استخدم [محلل الاتصال عن بُعد من Microsoft](https://testconnectivity.microsoft.com/) وقم بتشغيل **اختبارات اتصال خدمات الويب من Microsoft Exchange** للمستخدمين المتأثرين.

وأخيراً يمكنك التحقق من [تطبيقات Teams – نُهج إعداد التطبيقات](https://admin.teams.microsoft.com/policies/app-setup) للتأكد من أنه لم تتم إزالة تطبيق التقويم من النهج الذي تم تطبيقه على المستخدم (على الأرجح **العمومي (افتراضي على مستوى المؤسسة)**.

إذا كان المستخدمون يعملون في الأساس محلياً، فأنت بحاجة إلى التأكد من أن "التكوين المختلط" سليم. استخدم["معالج التكوين المختلط"](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent)لاستكشاف الأخطاء وإصلاحها.

تجدر الإشارة إلى أن [Teams يتطلب Exchange 2016 CU3 أو إصدار أحدث](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
