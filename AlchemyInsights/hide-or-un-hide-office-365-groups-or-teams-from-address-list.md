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
ms.openlocfilehash: 7e667e22cd81f38a1a2c1385bf42e5227cb641480f4b505110ee7349a13f13a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088383"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>إخفاء مجموعات أو فرق Office 365 أو إخفائها من قائمة العنوان

استخدم أمر EXO PowerShell التالي لإخفاء مجموعة/فرق Office 365 أو إخفائها من قوائم العنوان (GAL) لعملاء Exchange (Outlook، OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

استخدم أمر EXO PowerShell التالي لإخفاء مجموعة/فرق Office365 أو إخفائها من عملاء Exchange (Outlook، OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- للحصول على إرشادات مفصلة، راجع إخفاء Office 365 [من GAL Exchange العملاء](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).
