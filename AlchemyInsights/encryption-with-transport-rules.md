---
title: التشفير باستخدام قواعد النقل
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
- "9002635"
- "5154"
ms.openlocfilehash: e1f8227047daede71d0fa3b3557db0d95a379b99b76ab0c2fe1d6ed8cc213d4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079437"
---
# <a name="encryption-with-transport-rules"></a>التشفير باستخدام قواعد النقل

في [مركز إدارة Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC)، يمكنك استخدام إمكانيات "تشفير الرسائل من Office" (OME) في قواعد تدفق البريد لتشغيل تشفير الرسائل. اختر الخيار **تطبيق تشفير رسائل Office 365 وحماية الحقوق** في شرط "قاعدة النقل".

- للحصول على مزيد من المعلومات، راجع [تحديد قاعدة تدفق البريد للتشفير](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- في Powershell، استخدم cmdlet [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) وقم بتعيين المعلمة *ApplyOME* إلى $true.
