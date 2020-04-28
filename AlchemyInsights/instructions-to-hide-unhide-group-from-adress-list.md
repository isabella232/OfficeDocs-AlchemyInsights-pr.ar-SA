---
title: إرشادات لإخفاء/إلغاء إخفاء المجموعة من قائمة العناوين
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 61ba34e6d554831da712a92401f26fabb02c26b7
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908331"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>إخفاء مجموعة Microsoft 365 من قائمة العناوين (GAL)

لإخفاء مجموعة Microsoft 365 من قوائم العناوين (GAL) لعملاء Exchange (مثل Outlook أو OWA)، استخدم الأمر التالي في EXO shell:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

لإخفاء مجموعة Microsoft 365 من أن تكون مرئية لعملاء Exchange، استخدم الأمر التالي في EXO shell:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

