---
title: غير قادر علي حذف العناصر في SharePoint أو اندريف
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
ms.openlocfilehash: cc19fcb6603160032dac52b1ec9e194a90b7891f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049504"
---
# <a name="unable-to-delete-items"></a>غير قادر علي حذف العناصر

هل تواجه مشكلات في حذف عناصر SharePoint ؟

- تاكد دائما من ان لديك [الأذونات المناسبة](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) لحذف العنصر أو محاولة [مسؤول مجموعه موقع](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) أزاله العنصر.

- تاكد من عدم وجود اعداد [نهج استبقاء](https://docs.microsoft.com/office365/securitycompliance/retention-policies) علي العنصر.

- تاكد من عدم [سحب](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) العنصر إلى مستخدم آخر.

- وأخيرا ، يمكن للمسؤولين استخدام [أنماط SharePoint والممارسات](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) الذي يحتوي علي مكتبه من الأوامر PowerShell التي تسمح لك بتنفيذ إجراءات أداره معقده مثل فرض حذف العناصر العنيدة.
- [أزاله ملف PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [أزاله مجلد PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [أزاله عنصر قائمه PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [أزاله قائمه PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [أزاله حقل PNP (عمود)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)