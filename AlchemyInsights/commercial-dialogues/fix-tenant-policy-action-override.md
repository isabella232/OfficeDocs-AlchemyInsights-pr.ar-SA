---
title: إصلاح نهج المستأجر (تجاوز الإجراء)
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
ms.openlocfilehash: 157baa1f1e3f48b47ba07b8c6d446f8e081a4ad24b7d48f50c4fc5af5518cdd6
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896062"
---
# <a name="fix-tenant-policy-action-override"></a>إصلاح نهج المستأجر (تجاوز الإجراء)

لقد أثرت إحدى سياسات مكافحة البريد العشوائي على هذه الرسالة. لمراجعة السياسات، اتبع الخطوات التالية:

1. في مدخل Microsoft 365 Defender، انتقل إلى البريد الإلكتروني & سياسات التعاون & قواعد الحماية من البريد العشوائي في القسم <https://security.microsoft.com/>  \>  \>  \>  "سياسات". 

   انتقل مباشرة إلى صفحة **سياسات** مكافحة البريد العشوائي، استخدم <https://security.microsoft.com/antispam> .

2. في **صفحة نهج** مكافحة البريد العشوائي، حدد النهج بالنقر فوق اسم النهج  **(** النوع هو نهج مخصص لمكافحة البريد العشوائي أو الاسم **هو** نهج البريد الوارد لمكافحة البريد العشوائي **(افتراضي)**).
3. في الجزء منتحل التفاصيل الذي يظهر، حدد **تحرير الإجراءات** في **المقطع إجراءات.**
4. في القسم **إجراءات** الرسالة، راجع الأحكام الصادرة حول البريد العشوائي  والبريد العشوائي عالي الثقة والتصيد الاحتيالي والتصيد الاحتيالي عالي الثقة لمعرفة ما إذا تم تحديد أي من القيم التالية: 
   - **إضافة رأس X**
   - **سطر موضوع مع نص معتمد مسبقا**
   - **إعادة توجيه رسالة إلى عنوان البريد الإلكتروني**
   - **حذف رسالة**
   - **لا يوجد أي إجراء**

   من المحتمل أن  تكون الإعدادات القياسية المطبقة على جميع Exchange Online Protection قد تأثروا بالرسالة.

لمزيد من المعلومات، راجع تكوين سياسات مكافحة البريد العشوائي [في EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies).
