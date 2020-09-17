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
ms.openlocfilehash: fd12115214cc28b822cf7fa57fe9b86f76f7beb1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806098"
---
# <a name="unable-to-delete-items"></a>تعذر حذف العناصر

يمكن ان تتسبب نهج الاستبقاء بهذا الأمر ، ستحتاج إلى تعطيل التعليق أو استبعاده الذي يسبب هذه المشكلة. بعد أزاله نهج الاستبقاء أو التعليق ، قد تستغرق التغييرات حيز التنفيذ حتى 24 ساعة. تاكد من عدم وجود اعداد [نهج استبقاء](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) علي العنصر.

ربما تجاوز الموقع حد مساحة التخزين ، ويزيد [الحصة النسبية للموقع](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) ويحذف العنصر.

تاكد من [عدم سحب العنصر إلى مستخدم](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) آخر.

في النهاية ، يمكن للمسؤولين استخدام [أنماط وممارسات SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) التي تحتوي علي مكتبه لأوامر PowerShell التي تسمح لك بتنفيذ إجراءات الاداره المعقدة مثل فرض حذف العناصر الستوبورنه.
- [أزاله ملف PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [أزاله مجلد PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [أزاله عنصر قائمه PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [أزاله قائمه PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [أزاله حقل PNP (عمود)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)