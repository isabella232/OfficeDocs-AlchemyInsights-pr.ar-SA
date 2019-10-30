---
title: تعليمات لإخفاء/إظهار المجموعة من قائمه العناوين
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
ms.openlocfilehash: d0e0285701f1a5f308bdc682abaddf5cc2d34120
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768896"
---
# <a name="hide-office-365-group-from-address-list-gal"></a>إخفاء مجموعه 365 Office من قائمه العناوين (GAL)

لإخفاء مجموعه 365 Office من قوائم العناوين (GAL) من عملاء Exchange (مثل Outlook أو OWA) ، استخدم الأمر التالي في shell EXO:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

لإخفاء مجموعه 365 Office من ان تكون مرئية لعملاء Exchange ، استخدم الأمر التالي في shell EXO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

