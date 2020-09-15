---
title: إرشادات لإخفاء/إظهار المجموعة من قائمه العناوين
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 1ad9ab294d46ca0fc88a454e3503ddcf80398896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662996"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>إخفاء مجموعه Microsoft 365 من قائمه العناوين (GAL)

لإخفاء مجموعه Microsoft 365 من قوائم العناوين (GAL) لعملاء Exchange (مثل Outlook أو OWA) ، استخدم الأمر التالي في أكسو shell:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

لإخفاء مجموعه Microsoft 365 من ان تكون مرئية لعملاء Exchange ، استخدم الأمر التالي في أكسو shell:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

