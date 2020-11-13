---
title: تعذر حذف العناصر في SharePoint أو OneDrive
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
ms.openlocfilehash: db45aa8df40484fdcda7c430f1ca27482a1dd4ce
ms.sourcegitcommit: a9415f3ae8c7ba267b5134bcbdc1e070cea41a0f
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/12/2020
ms.locfileid: "49019570"
---
# <a name="unable-to-delete-items"></a>تعذر حذف العناصر

- يمكن ان تتسبب نهج الاستبقاء بهذا الأمر ، ستحتاج إلى تعطيل التعليق أو استبعاده الذي يسبب هذه المشكلة. بعد أزاله نهج الاستبقاء أو التعليق ، قد تستغرق التغييرات حيز التنفيذ حتى 24 ساعة. تاكد من عدم وجود اعداد [نهج استبقاء](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) علي العنصر.

- ربما تجاوز الموقع حد مساحة التخزين ، ويزيد [الحصة النسبية للموقع](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) ويحذف العنصر.

- تاكد من [عدم سحب العنصر إلى مستخدم](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) آخر.

- في النهاية ، يمكن للمسؤولين استخدام [أنماط وممارسات SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) التي تحتوي علي مكتبه لأوامر PowerShell التي تسمح لك بتنفيذ إجراءات الاداره المعقدة مثل فرض حذف العناصر الستوبورنه.
- [أزاله ملف PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [أزاله مجلد PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [أزاله عنصر قائمه PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [أزاله قائمه PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [أزاله حقل PNP (عمود)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)