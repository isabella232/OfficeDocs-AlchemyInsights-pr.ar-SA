---
title: غير قادر على حذف عناصر SharePoint أو أندريف
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: d25214f26a3168e3e350b5cc31ca870e65d48ad9
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/28/2019
ms.locfileid: "35366520"
---
# <a name="unable-to-delete-items"></a>غير قادر على حذف العناصر

تواجه مشكلات حذف العناصر؟

- تأكد دائماً لديك [الأذونات المناسبة](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) لحذف العنصر أو محاولة [مسؤول مجموعة الموقع](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) إزالة العنصر.

- تأكد من أنه لا يوجد إعداد [نهج الاستبقاء](https://docs.microsoft.com/office365/securitycompliance/retention-policies) على العنصر.

- تأكد من أن العنصر ليس [قيد السحب](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) إلى مستخدم آخر.

- وأخيراً، يمكن للمسؤولين استخدام [أنماط SharePoint والممارسات](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) الذي يحتوي على مكتبة PowerShell الأوامر التي تسمح لك بتنفيذ إجراءات إدارة معقدة مثل فرض حذف العناصر العنيدة.
- [إزالة ملف PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [إزالة المجلد PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [إزالة عنصر قائمة PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [إزالة قائمة PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [إزالة PNP حقل (عمود)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)