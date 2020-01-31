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
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571212"
---
# <a name="unable-to-delete-items"></a>غير قادر على حذف العناصر

يمكن أن تتسبب نُهج الاحتفاظ في حدوث ذلك، تحتاج إما إلى تعطيل أو استبعاد احتجاز كل منهما الذي يسبب هذه المشكلة. بعد إزالة نهج الاحتفاظ أو الانتظار، قد يستغرق الأمر ما يصل إلى 24 ساعة حتى يسري التغيير. تأكد من عدم وجود إعداد [نهج الاحتفاظ](https://docs.microsoft.com/office365/securitycompliance/retention-policies) على العنصر.

قد يكون الموقع قد تجاوز حد التخزين وزيادة [حصة الموقع وحذف](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) العنصر.

تأكد من عدم [سحب](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) العنصر إلى مستخدم آخر.

وأخيراً، يمكن للمسؤولين استخدام [أنماط وممارسات SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) التي تحتوي على مكتبة من أوامر PowerShell التي تسمح لك بتنفيذ إجراءات إدارة معقدة مثل فرض حذف العناصر العنيدة.
- [إزالة ملف PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [إزالة مجلد PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [إزالة عنصر قائمة PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [إزالة قائمة PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [إزالة حقل PNP (عمود)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)