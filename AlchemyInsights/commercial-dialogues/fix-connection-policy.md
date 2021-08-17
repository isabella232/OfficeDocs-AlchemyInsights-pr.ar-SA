---
title: إصلاح نهج الاتصال
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
ms.openlocfilehash: 9094dcdc4507f52da1dd7c95f83aa98bab1446639d2d9f52eb3a7bc849dc183c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/11/2021
ms.locfileid: "57888393"
---
# <a name="fix-connection-policy"></a>إصلاح نهج الاتصال

تم وضع علامة آمن على البريد الإلكتروني وتسليمه إلى علبة وارد المستخدم لأنه تم وضع علامة على عنوان IP المصدر كآمن في نهج تصفية الاتصال الافتراضي. لمراجعة النهج، اتبع الخطوات التالية:

1. في مدخل Microsoft 365 Defender في ، انتقل إلى البريد الإلكتروني & سياسات التعاون & قواعد الحماية من البريد العشوائي في القسم <https://security.microsoft.com/>  \>  \>  \>  "سياسات". 

   انتقل مباشرة إلى صفحة **سياسات** مكافحة البريد العشوائي، استخدم <https://security.microsoft.com/antispam> .

2. في صفحة **نهج مكافحة البريد** العشوائي، حدد النهج المسمى نهج تصفية الاتصال **(افتراضي)** بالنقر فوق اسم النهج.

3. في القائمة flyout التفاصيل التي تظهر، انقر فوق **تحرير نهج تصفية الاتصال** في المقطع تصفية **الاتصال.**

4. راجع الإدخالات في المقطع السماح دائما بالرسائل من عناوين **IP**  أو نطاق العناوين التالية، وراجع ما إذا تم تحديد تشغيل القائمة الآمنة.

   > [!NOTE]
   > تشترك Microsoft في مصادر جهة خارجية للمرسلين الموثوق بهم. إذا تم تمكين القائمة الآمنة، لا يتم وضع علامة عن طريق الخطأ على هؤلاء المرسلين الموثوق بهم كرسالة عشوائية. نوصي بتحديد هذا الخيار، لأنه سيقلل عدد الإيجابيات الخاطئة (البريد الجيد المصنف كبريد عشوائي) الذي تتلقاه.

لمزيد من المعلومات، راجع [تكوين تصفية الاتصال](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy).
