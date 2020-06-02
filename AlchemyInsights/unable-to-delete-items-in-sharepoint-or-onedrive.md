---
title: غير قادر على حذف العناصر في SharePoint أو OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 8647b65c52a782ca48ca58bb2700556db528796b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511963"
---
# <a name="unable-to-delete-items"></a>غير قادر على حذف العناصر

يمكن أن تتسبب نُهج الاحتفاظ في ذلك، تحتاج إما إلى تعطيل أو استبعاد الاحتفاظ المعني الذي يسبب هذه المشكلة. بعد إزالة سياسة الاحتفاظ أو الانتظار، قد يستغرق التغيير ما يصل إلى 24 ساعة حتى يدخل التغيير حيز التنفيذ. تأكد من عدم وجود إعداد [نهج الاحتفاظ](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) على العنصر.

قد يكون الموقع قد تجاوز حد التخزين وزيادة [حصة الموقع النسبية](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) وحذف العنصر.

تأكد من عدم [سحب](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) العنصر إلى مستخدم آخر.

وأخيراً، يمكن للمسؤولين استخدام [أنماط وممارسات SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) التي تحتوي على مكتبة من أوامر PowerShell التي تسمح لك بتنفيذ إجراءات إدارة معقدة مثل فرض حذف العناصر العنيدة.
- [إزالة ملف PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [إزالة مجلد PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [إزالة عنصر قائمة PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [إزالة قائمة PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [إزالة حقل PNP (عمود)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)