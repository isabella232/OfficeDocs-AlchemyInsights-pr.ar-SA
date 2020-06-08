---
title: إخفاء مجموعات أو فرق Office 365 أو إلغاء إخفائها من قائمة العناوين
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: cb3c2819ff7203774511bd0e45633b59a02091ff
ms.sourcegitcommit: e3a1f96200bc58dc8a5b3597cc2600e71c4bd266
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/14/2020
ms.locfileid: "44225311"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>إخفاء مجموعات أو فرق Office 365 أو إلغاء إخفائها من قائمة العناوين

استخدم الأمر التالي EXO PowerShell لإخفاء أو إلغاء إخفاء مجموعة/فرق Office 365 من قوائم العناوين (GAL) لعملاء Exchange (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

استخدم الأمر التالي EXO PowerShell لإخفاء أو إلغاء إخفاء مجموعة/فرق Office365 من عملاء Exchange (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- للحصول على تعليمات مفصلة، راجع [إخفاء مجموعات Office 365 من عملاء GAL و Exchange](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).
