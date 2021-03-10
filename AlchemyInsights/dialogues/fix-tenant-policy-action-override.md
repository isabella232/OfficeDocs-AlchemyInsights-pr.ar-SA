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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692497"
---
# <a name="fix-tenant-policy-action-override"></a>إصلاح نهج المستأجر (تجاوز الإجراء)

لقد تأثر نهج مكافحة البريد العشوائي في المستأجر بهذه الرسالة. لمراجعة النهج، يمكنك القيام بما يلي:

1. انتقل إلى مركز التوافق & الأمان في [Office 365،](https://go.microsoft.com/fwlink/p/?linkid=2077143)ثم انتقل إلى نهج إدارة المخاطر   >    >  [لمكافحة البريد العشوائي.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. تحقق لمعرفة ما إذا كان مصدر **النهج** يشير إلى ما  **يلي: Add-Xheader/ModifySubject/Redirect/Delete/No action/BCC رسالة**

    إذا كان الأمر  كذلك، فتحقق من إعدادات النهج الذي تأثر بالرسالة على علامة التبويب "مخصص". من المحتمل أن تكون الإعدادات القياسية **المطبقة** على كل عملاء Exchange Online Protection قد أثرت على الرسالة.

لمزيد من المعلومات حول تكوين سياسات تصفية البريد العشوائي، راجع ["تكوين سياسات](https://go.microsoft.com/fwlink/?linkid=2101431)تصفية البريد العشوائي".
