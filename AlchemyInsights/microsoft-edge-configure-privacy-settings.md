---
title: Microsoft Edge تكوين إعدادات الخصوصية
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/08/2020
ms.locfileid: "49676709"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge تكوين إعدادات الخصوصية

بشكل افتراضي ، إذا تم نشر Microsoft Edge علي الانظمه الاساسيه غير التابعة لنظام التشغيل Windows ، فلن يتم إرسال البيانات التشخيصية ومعلومات الموقع إلى Microsoft. ومع ذلك ، إذا تم نشر Microsoft Edge علي Windows 10 ، سيتم إرسال بيانات التشخيص ومعلومات الموقع وفقا [لإعدادات بيانات تشخيص Windows](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)الخاصة بالمستخدمين.

لتكوين الطريقة التي يتعامل بها Microsoft Edge مع مجموعه البيانات لمؤسسك ، استخدم نهج المجموعة التالية:
- [ميتريكسريبورتينجينابليد](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): يؤدي هذا النهج إلى تمكين اعداد تقارير الاستخدام والبيانات ذات الصلة بالعطل.
- [سيندسيتينفوتويمبروفيسيرفيسيس](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): يقوم هذا النهج بإرسال معلومات الموقع المستخدمة لتحسين خدمات Microsoft.

لمعرفه المزيد ، راجع [تكوين إعدادات النهج](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).