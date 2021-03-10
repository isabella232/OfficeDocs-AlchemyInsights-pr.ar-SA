---
title: مثال على نهج المرفق الآمن ل Microsoft Defender ل Office 365
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
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692458"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>مثال على نهج المرفق الآمن ل Microsoft Defender ل Office 365

تمكن هذه الإعدادات  نهج يسمى "لا توجد تأخيرات" التي تقوم بتسليم الرسائل على الفور ثم إعادة إرفاق المرفقات بعد فحصها:

- **الاسم:** لا توجد تأخيرات
- **الوصف:** يتم تسليم الرسائل على الفور ثم إعادة إرفاق المرفقات بعد الفحص.
- **الاستجابة:** حدد **خيار التسليم الديناميكي.** لمزيد من المعلومات، راجع [التسليم الديناميكي في سياسات المرفقات الآمنة.](https://go.microsoft.com/fwlink/?linkid=2092328)
- **قسم "إعادة** توجيه المرفقات": حدد الخيار "تمكين إعادة التوجيه"، ثم أدخل عنوان البريد الإلكتروني لمسؤول Microsoft 365 العام أو مسؤول الأمان أو محلل الأمان الذي سيتحقق من المرفقات الضارة. 
- **القسم "مطبق** على": **حدد مجال المستلم،** ثم حدد مجالك. حدد **"إضافة"،** ثم حدد **"موافق".** بمجرد الانتهاء، حدد **"حفظ".**

لمعرفة المزيد، راجع ["المرفقات الآمنة" في Microsoft Defender ل Office 365.](https://go.microsoft.com/fwlink/?linkid=2092213)
