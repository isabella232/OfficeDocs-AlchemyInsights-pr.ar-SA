---
title: يتعذر حذف العناصر في SharePoint أو OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3601c5eff121e10b6bddace6f7228204a01080a636e24f3a56373fe8d469c799
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038504"
---
# <a name="unable-to-delete-items"></a>تعذر حذف العناصر

- قد تتسبب سياسات الاستبقاء في حدوث ذلك، ستحتاج إما إلى تعطيل احتجاز كل واحد أو استبعاده مما يتسبب في هذه المشكلة. بعد إزالة نهج الاستبقاء أو الاستمرار، قد يستغرق الأمر ما يصل إلى 24 ساعة حتى يتم إجراء التغيير. تأكد من عدم وجود إعداد نهج [استبقاء](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) على العنصر.

- من المحتمل أن يكون الموقع قد تجاوز الحد الأقصى للتخزين وزيادة [الحصة](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) النسبية للموقع وحذف العنصر.

- تأكد من عدم سحب [العنصر إلى](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) مستخدم آخر.

- وأخيرا، يمكن للمسؤولين [](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) استخدام SharePoint الأنماط والممارسات (PnP) التي تحتوي على مكتبة لأوامر PowerShell التي تسمح لك بتنفيذ إجراءات إدارة معقدة مثل فرض حذف عناصر غير مهمة.
- [إزالة ملف PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [إزالة مجلد PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [إزالة عنصر قائمة PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [إزالة قائمة PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [إزالة حقل PNP (عمود)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)