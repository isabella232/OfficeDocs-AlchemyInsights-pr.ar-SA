---
title: تجمع الترحيل الصادر
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: 7e5bb1fda1dec0c0f72d1944d54b6f2747a6e909
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326064"
---
# <a name="outbound-relay-pool"></a>تجمع الترحيل الصادر

تقوم Microsoft بإجراء بعض التغييرات على التكوين لترحيل البريد الإلكتروني أو إعادة توجيهه عبر Microsoft 365. يتم إعادة توجيه الرسائل في سيناريوهات معينة أو ترحيلها Microsoft 365 باستخدام تجمع ترحيل خاص. قد تنتهي الرسائل المرسلة باستخدام تجمع الترحيل في مجلد البريد غير الهام الخاص بالمستلم. لمزيد من المعلومات، راجع [تجمعات تسليم الصادرات](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

لتجنب سيناريو باستخدام تجمع الترحيل، تأكد من أن الرسائل التي تم إعادة توجيهها/ترحيلها تلبي أحد المعايير التالية:

- المرسل الصادر هو مجال مقبول للمستأجر.
- يتم تمرير إطار نهج المرسل (SPF) عندما تظهر الرسالة Microsoft 365.
- يتم تمرير DomainKeys Identified Mail (DKIM) على مجال مرسل P2 عندما تظهر الرسالة Microsoft 365.
 
لا يتم ترحيل الرسائل التي تفي بالمعايير أعلاه عبر تجمع الترحيل.

إذا كان سجل MX لمجالك مشارا إلى خادم جهة خارجية أو خادم داخلي، فاستخدم التصفية المحسنة للتأكد من صحة التحقق من صحة SPF للبريد الإلكتروني الوارد ولتجنب إرسال البريد الإلكتروني عبر تجمع الترحيل.

**كيف يمكننا معرفة ما إذا كان تجمع الترحيل متأثيا؟**

إذا كانت رسائل البريد الإلكتروني التي تم إعادة توجيهها أو ترحيلها تستخدم أحد المعايير أعلاه، فلن يتم ترحيل الرسائل عبر تجمع الترحيل. ومع ذلك، إذا تم إرسال رسالة عبر تجمع ترحيل، فإن IP للخادم الصادر يكون في النطاق 40.95.0.0/16 ويتضمن اسم الخادم الصادر **rly** في الاسم.

