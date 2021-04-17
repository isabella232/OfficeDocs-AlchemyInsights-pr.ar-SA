---
title: إرشادات لإخفاء/إخفاء المجموعة من قائمة العنوان
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 4d55866700b9b8494f1f692cd3b865116b96a1bc
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831865"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>إخفاء مجموعة Microsoft 365 من قائمة العنوان (GAL)

لإخفاء مجموعة Microsoft 365 من قوائم العنوان (GAL) لعملاء Exchange (مثل Outlook أو OWA)، استخدم الأمر التالي في EXO shell:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

لإخفاء مجموعة Microsoft 365 حتى لا تكون مرئية لعملاء Exchange، استخدم الأمر التالي في EXO shell:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

