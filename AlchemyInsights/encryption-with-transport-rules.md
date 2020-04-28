---
title: التشفير باستخدام قواعد النقل
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: 3f16c7e7be99a50cd57f47ea2801b3022c4aec95
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915005"
---
# <a name="encryption-with-transport-rules"></a>التشفير باستخدام قواعد النقل

في [مركز إدارة Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC)، يمكنك استخدام إمكانيات "تشفير الرسائل من Office" (OME) في قواعد تدفق البريد لتشغيل تشفير الرسائل. اختر الخيار **تطبيق تشفير رسائل Office 365 وحماية الحقوق** في شرط "قاعدة النقل".

- للحصول على مزيد من المعلومات، راجع [تحديد قاعدة تدفق البريد للتشفير](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- في Powershell، استخدم cmdlet [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) وقم بتعيين المعلمة *ApplyOME* إلى $true.
