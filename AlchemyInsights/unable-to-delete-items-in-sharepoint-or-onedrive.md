---
title: غير قادر على حذف عناصر SharePoint أو أونيدريفي
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 21d7b928fade48a6729c120e6ea33b16dafe799e
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057664"
---
# <a name="unable-to-delete-items"></a>غير قادر على حذف العناصر

تواجه مشكلات حذف العناصر؟

- تأكد دائماً لديك [الأذونات المناسبة](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) لحذف العنصر أو محاولة [مسؤول مجموعة الموقع](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) إزالة العنصر.

- تأكد من أنه لا يوجد إعداد [نهج الاستبقاء](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) على العنصر.

- تأكد من أن العنصر ليس [قيد السحب](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) إلى مستخدم آخر.

- وأخيراً، يمكن للمسؤولين استخدام [أنماط SharePoint والممارسات](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) الذي يحتوي على مكتبة PowerShell الأوامر التي تسمح لك بتنفيذ إجراءات إدارة معقدة مثل فرض حذف العناصر العنيدة. 
- [إزالة ملف PNP](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [إزالة المجلد PNP](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [إزالة عنصر قائمة PNP](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [إزالة قائمة PNP](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [إزالة PNP حقل (عمود)](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)