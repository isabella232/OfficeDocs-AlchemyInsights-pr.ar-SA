---
title: إخفاء مجموعات أو فرق Office 365 أو إخفائها من قائمة العنوان
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
- "9002947"
- "5642"
ms.openlocfilehash: 12e221c69775f3dfeed1781b70d3061e1ca0ac3b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811443"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>إخفاء مجموعات أو فرق Office 365 أو إخفائها من قائمة العنوان

استخدم الأمر التالي EXO PowerShell لإخفاء مجموعة/فرق Office 365 أو إخفائها من قوائم العنوان (GAL) لعملاء Exchange (Outlook، OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

استخدم الأمر التالي EXO PowerShell لإخفاء مجموعة/فرق Office365 أو إخفائها من عملاء Exchange (Outlook، OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- للحصول على إرشادات مفصلة، راجع [إخفاء مجموعات Office 365 من GAL والعملاء من Exchange](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).
